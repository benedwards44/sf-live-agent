# sf-live-agent
Simple HTML sample page for testing Live Agent with Salesforce. You can load this locally on your machine, or load it as a static website on AWS S3 or any server.

## Quick Setup

I've recommend following the Salesforce Live Agent setup for more detailed instructions:
https://developer.salesforce.com/docs/atlas.en-us.workbook_service_cloud.meta/workbook_service_cloud/service5_step1.htm

But here's the quick, simple setup:

1. Create a Skill 
2. Create a Live Agent Deployment in Salesforce (take note of the Deployment Id)
3. Create a Live Agent Configuration in Salesforce
4. Create a Live Agent Chat Button in Salesforce (take note of the Button Id)
5. In the index.html file, replace BUTTONID, ORGID and DEPLOYMENTID with values created above

If you load the index.html file, it should display that Chat is Offline. You will need to login to Salesforce as an Agent User and be online. These steps are required:

1. Enable a user as a Live Agent User
2. Enable a user as a Service Cloud User
3. Add a Service (or Sales) Console license as a Permission Set License Assignment
4. Create a Console App (if not done already), and enable the Console App as supporting Live Agent.
5. Open the Console App, click Live Agent down the bottom right and mark yourself as Online.
6. Load the index.html file (or website where it's hosted), and you should now be able to start a chat.
