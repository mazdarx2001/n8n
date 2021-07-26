---
permalink: /credentials/ciscoWebex
description: Learn to configure credentials for the Cisco Webex node in n8n
---

# Cisco Webex

You can use these credentials to authenticate the following nodes:
- [Cisco Webex](../../nodes-library/nodes/ciscoWebex/README.md)
- [Cisco Webex Trigger](../../nodes-library/trigger-nodes/ciscoWebexTrigger/README.md)

## Prerequisites

Create a [Cisco Webex](https://www.webex.com/) account.

## Using OAuth

1. Navigate to [Webex for Developers](https://developer.webex.com/) and sign in using your Cisco Webex account.
2. From the user menu select **My Webex Apps**, then **Create a New App**.
3. From the ***Create a New App*** page select **Create an Integration**.
4. Complete the following required fields for your new integration:
    * ***Integration Name***: Provide a name for your Webex app.
    * ***Contact Email***: Enter your email address.
    * ***Icon***: Provide an icon for your app or select one of the available defaults.
    * ***Description***: Enter a brief description of your app.
    * ***Redirect URIs***: Enter the **OAuth Callback URL** from the n8n credentials modal.
    * ***Scopes***: Select the access granted to your new app.
5. Click **Add Integration** to create your app.
6. Copy the ***Client ID*** and ***Client Secret*** for this new app.

From n8n:

7. Enter a descriptive ***Credentials Name***.
8. Under ***Credential Data***, enter the ***Client ID*** and ***Client Secret*** obtained above.
9. Under ***OAuth***, click the circle button to initiate authentication. A popup may appear prompting you to login to your Cisco Webex account.
10. After authentication is complete, click **Create** to save your new credentials.
