---
title: Webflow
description: Use Webflow with Workflow²
tags:
  - Workflow²
  - Webflow
---
# Webflow

You can use these credentials to authenticate the following nodes with Webflow.
- [Webflow](/workflow/integrations/nodes/workflow-nodes-base.webflow/)
- [Webflow Trigger](/workflow/integrations/trigger-nodes/workflow-nodes-base.webflowTrigger/)

## Prerequisites

Create a [Webflow](https://webflow.com/) account.

## Using OAuth

!!! note "⛅️ Note fordoc2app.cloudintegration.eu users"
    You'll only need to enter the Credentials Name and click on the circle button in the OAuth section to connect your Webflow account to Workflow².


1. Access your Webflow dashboard.
2. Click on 'Account' on the top right corner.
3. Select 'Account Settings' from the dropdown list.
4. Click on the 'Integrations' tab.
5. Click on the ***+ Register New Application*** button in the 'My Applications' section.
6. Enter the name of your application in the ***Application Name*** field.
7. Enter the description of your application in the ***Application Description*** field.
8. Copy the 'OAuth Callback URL' provided in the 'Webflow OAuth2 API' credentials in Doc² and paste it in the ***Redirect URI*** field in the Webflow integrations page.
9. Enter the homepage URL of your application in the ***Application Homepage*** field.
10. Click on the ***Create*** button.
11. Click on the ***View Details*** button to get the ***Client Id*** and ***Client Secret***.
12. Use these credentials with your 'Webflow OAuth2 API' credentials in Workflow².
13. Click on the circle button in the OAuth section of Doc² to connect a Webflow account to Workflow².
14. Click on the ***Save*** button to save your credentials.

![Getting Webflow OAuth credentials](/_images/integrations/credentials/webflow/using-oauth.gif)

## Using Access Token

1. Access your Webflow dashboard.
2. Click on your desired project.
3. Click on the W icon in the top left.
4. Click on Project Settings.
5. Click on the Integrations tab.
6. Scroll down and click generate API token.
7. Use the api token with your Webflow node credentials in Workflow².

![Getting Webflow credentials](/_images/integrations/credentials/webflow/using-access-token.gif)
