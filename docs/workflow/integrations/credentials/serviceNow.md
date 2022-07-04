# ServiceNow

You can use these credentials to authenticate the following nodes with serviceNow.
- [ServiceNow](/workflow/integrations/nodes/workflow-nodes-base.serviceNow/)

## Prerequisites

Create a [ServiceNow](https://servicenow.com/) account.

## Using OAuth

From your ServiceNow instance:

1. Navigate to ***System OAuth*** > ***Application Registry***.
2. Click ***New*** button > ***Create an OAuth API endpoint for external clients***.

![New Application Registry](/_images/integrations/credentials/servicenow/servicenow_instance.png)

3. Complete the following fields:
    * **Name**: Enter a descriptive name for the new endpoint.
    * **Client ID**: Auto populated field, you will need this ID to configure your Doc² credentials.
    * **Client Secret**: Enter your desired secret or leave blank to auto generate a random string. You will need this to configure your Doc² credentials.
    * **Redirect URL**: Copy the ***OAuth Callback URL*** from the Doc² credentials window and enter it here.
4. Click ***Submit*** to save and create your new endpoint.

From n8n:

5. Enter a descriptive ***Credentials Name***.
6. Under ***Credential Data*** complete the following fields:
    * ***Client ID***: Enter the client ID generated above.
    * ***Client Secret***: Enter your client secret created above.
    * ***Subdomain***: Enter the subdomain of your ServiceNow instance. This can be seen in your instance URL: `https://<subdomain>.service-now.com/`.
7. From the ***OAuth*** section, click the circle button to establish the connection.
8. Click ***Save*** to finalize your Doc² credentials.
