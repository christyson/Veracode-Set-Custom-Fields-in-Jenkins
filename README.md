# Veracode-Set-Custom-Fields-in-Jenkins
A snippet for a Jenkins pipeline to set both Application and Sandbox level custom fields for use with the Jira integration.

See the file for the snippet.  It relies on the following variables for usw with a pipeline with build parameters:

  VC_ProjectName:         	<your Veracode project name>
  VERACODE_WRAPPER_VERSION: set to the latest release number of the Veracode Java Wrapper (currently: 19.11.6.0) 
                            can be found here https://help.veracode.com/reader/LMv_dtSHyb7iIxAQznC~9w/OwyjPkzVaNJWGh7IPPF1OQ
  SandboxName:            	<your sandbox name if you are using one>
  CustomField:            	Custom field name you want to set typically Custom 1
  JiraProjectName:          <the name of your project in Jira>

Note: assumes your Jenkins script can use java, grep and td.
