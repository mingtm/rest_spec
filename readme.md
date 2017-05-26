# MS Graph REST API Docs Template Generator

This guide provides instructions to take a XML CSDL file and generate API and resource shell/tempalte for the purpose of documenting the APIs. This process does not account for the descriptions/information already available in the beta and v1.0 repositories. 

## Scenario and Usage 

If a new API/resource been introduced to your workload <or> a large scale update needs to be made to existing API docs, then regeneration of API shell/templates might be useful rather than manually creating the API docs. If you have a small change to be made (e.g., updating descriptions, adding scopes, adding examples, etc.) then do not use this tool. 

Usage: 

* Generate the shell/template. 
* Perform updates (add descriptions, examples, etc.) and merge any changes from the beta or v1.0 branches of the MS Graph docs repo. 
* Send a pull request to the beta/v1.0 branches of the MS Graph repo. 

## Pre-requisites to run this tool
Ruby interpreter. Version 2.1+
On windows machine, update PATH environment variable to point to ryby.exe file so you can run the command from any directory. 

Type `ruby -v` command to ensure that it is installed and working correctly. 

#### Install activesupport gem
This is required to parse XML file. 
Type `gem install activesupport` on command line. 

You should be set to go.. 


## Tool Setup

1. **Fork** this repository to your own GitHub account. If you already have a copy, please discard and fork fresh to get latest updates. 
1. Change directory to `rest_spec/lib` folder.
1. Open `edmx2json.rb` file. Update the XML location in the line: `f  = Net::HTTP.get(URI.parse('https://graph.microsoft.com/v1.0/$metadata'))`
1. If you run into SSL issues, just download the XML file locally and store the XML file into `/data` folder under the name `metadata.xml` and comemnt the above line and uncomment the below line: `f = File.read('../data/metadata.xml', :encoding => 'UTF-8')
`. This will ensure that file is read locally and you don't have to go over the network. 
1. Create a folder called logs on the same level as `rest_spec` folder. 
1. Run `ruby edmx2json.rb` command to generate intermediary JSON files. This takes more than 1-min to 3-hours (depending on the size of XML file) to complete. 
1. Run `ruby json2md.rb` command to generate markdonw files. It can take 1-15 minutes.
1. Find your Markdown templates in the `rest_spec/markdowns` folder. 
1. If you need to run the tool for different versions, save the markdowns/ folder content elsewhere. 
1. Copy the API/resource files to MS Graph fork local copy folders to make your edits. 

## Edit spec files

Add rich descriptions to the generated documentation to help our customers make sense of huge amount of APIs that are being enabled through Microsoft Graph. 

The process is simple and should be familiar to everyone at this point. Simply find the file you wish to edit (entity types are in the *resources/* folder and actions/functions including create/update/delete APIs are in the *api/* folder) and edit the Markdown. 

Key things to consider: 

* Add object, property, method, and parameter descriptions. 
* NOTE: Same descriptions can appear in many places. For example, the method descriptions appear in object Tasks table and also in the API file itself. Same object can appear as a relationship in many places. The descriptions that we add should be consistent across these locations.
* For APIs, add the **scopes** needed under the prerequisites section.
* For APIs, verify/edit HTTP request. There are hundreds of ways to reach the resource/methods through various resource paths. We have selected only a few for brevity. Add the ones that you wish to highlight. 
* For APIs, add the HTTP header details (optional or required). The template has a placeholder. If no HTTP headers are used, remove the sub-section. 
* Add any additional details required around HTTP request/response. 
* Format the response payload (JSON) as you wish. If you want to only show few properties to brevity, set the `truncated` flag in the comments (which is right above the response) to true. 
* Format the resource JSON representation as you wish. 
* The generator makes assumption about the response codes. Verify HTTP response code is what is actually being returned in the API. 
* Note that ComplexTypes are also shown as a resource. These files don't have Tasks section. 
* If you need to add any new methods (such as PUT API), following these steps
** Add an entry in the resource's Tasks table. 
** Add a new file: `resource_methodname.md` and include API details. 
** Ensure all the links work correctly.

Note:
* Do not change the file name. 
* Do not move the property, relationship, or tasks tables. 
* Refrain from adding new column to the table. 


### Formatting guidelines

In an effort to keep our documentation uniform with the same look and feel across all of it, please adhere to the following guidelines:

* For subheadings, use `###` followed by a space and then your heading text. Don't add any new subheadings unless the existing template doesn't cover the topic you wish to add. 
* To bold text, use `**text**`.
* To italicize text, use `*text*`.
* To add code snippets, use fences (```) and specify a coding language.
* Don't use newlines in tables. It just doesn't work.

## Submit a pull request

All changes need to eventually needs to end up in `master` branch of the repositiry. However, we don't update the master directly. The correct sequence is to update the `beta` and/or `v1.0` (depending on where the change needs to occur) and then update the `master` branch using a separate pull-request. 

So, you'd need multiple pull request to ensure that changes get reflected to master branch. 

Update Sequence:  

1. Fork and clone https://github.com/OfficeDev/microsoft-graph-docs  
2. Switch to `staging` branch first
3. Perform edits under your account. Make the relevant changes under `/beta` and/or `v1.0` folder of the reference content
4. Send pull requests to merge your changes  
5. Check the appVeyor status after you create Pull Request. If there is an error, cancel the pull request and fix the underlying issue before submitting the next pull request  

Note
* Do not push changes under /officedev account directly. 
* Do not push changes to master directly before updating `staging` branch.

### AppVeyor errors: 

When you submit PR, you may get validation errors. Some of known issues with the templates files are: 

* Many APIs return string/boolean values (scalars). Looks like the scaler return types are not supported in markdown scanner tool yet. Ignore errors that say `Unable to locate a definition for resource type: <type such as string or boolean>` for the time being. 
* The casing of object types are case-sensitive. `"@odata.type": "microsoft.graph.audiotrack"` and `"@odata.type": "microsoft.graph.audioTrack"` are treated differently. If you find resource not found errors, check the casing of the @odata.type in the resource file to make sure the casing is right (should be camel case). 

There may be others... Go through each of the error and fix them prior to proceeding. Any PR with errors can't be merged. 

## TOC (Table of Content on graph.microwsoft.io website) 
Contact us if you need updates to update TOC changes. 

## ADVANCED: Run Markdown Scanner tool locally for large set of changes

If you make a LOT of changes, it is worth considering running markdown scanner locally to avoid having to understand issues through the Github PR. the tool [markdown scanner](https://github.com/OneDrive/markdown-scanner) can be downloaded and setup locally. 

If you face any issues in running the tool, let us know.

### to run the scanner 

C:\Windows\Microsoft.NET\Framework64\v4.0.30319\msbuild MarkdownScanner.sln 

\markdown-scanner\ApiDocs.Console\bin\Debug>apidocs check-docs --path ..\..\rest_spec\markdowns


## Questions or concerns

Please log an issue on the repo.
