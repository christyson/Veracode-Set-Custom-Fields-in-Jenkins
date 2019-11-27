# Veracode-Set-Custom-Fields-in-Jenkins
A snippet for a Jenkins pipeline to set both Application and Sandbox level custom fields for use with the Jira integration.

See the [snippet](https://github.com/christyson/Veracode-Set-Custom-Fields-in-Jenkins/blob/master/Veracode%20Set%20Custom%20Field%20Snippet).  It relies on the following variables for usw with a pipeline with build parameters:
<pre><code>
1. VC_ProjectName:            your Veracode project name
2. VERACODE_WRAPPER_VERSION:  set to the latest release number of the Veracode Java Wrapper (currently: 19.11.6.0) 
3. SandboxName:               your sandbox name if you are using one
4. CustomField:               Custom field name you want to set typically Custom 1
5. JiraProjectName:           the name of your project in Jira
</pre></code>

####  Notes: 

- Information about the  Veracode wrapper version can be found can be found [here](https://help.veracode.com/reader/LMv_dtSHyb7iIxAQznC~9w/OwyjPkzVaNJWGh7IPPF1OQ)
- The Veracode wrapper version can be found can be found [here](https://search.maven.org/search?q=a:vosp-api-wrappers-java)
- The snippet assumes your Jenkins script can use java, grep and td. 
