
---
title: HubSpot
description: You can use these credentials to authenticate the following nodes with HubSpot.
tags:
  - Workflow²
  - HubSpot
---

# HubSpot

You can use these credentials to authenticate the following nodes with HubSpot.
- [HubSpot](/workflow/integrations/nodes/workflow-nodes-base.hubspot/)
- [HubSpot Trigger](/workflow//integrations/trigger-nodes/workflow-nodes-base.hubSpotTrigger/)

## Prerequisites

Create a [HubSpot](https://www.hubspot.com/) account.

## Using OAuth

!!! note "⛅️ Note fordoc2app.cloudintegration.eu users"
    You'll only need to enter the Credentials Name and click on the circle button in the OAuth section to connect your HubSpot account to Workflow².


!!! warning "⚠ HubSpot old accounts"
    Some HubSpot accounts don't have access to all the scopes. HubSpot is migrating accounts gradually. If you can't' find all the scopes in your current HubSpot developer account, try creating a fresh developer account.


1. Access your [HubSpot Developer Home](https://developers.hubspot.com/).
2. Click on the **Manage apps** button.
3. Click on the **Create app** button in the top right.
4. Specify an app name in the **Public app name** field.
5. Click on the 'Auth' tab.
6. Use the provided **Client ID** and the **Client secret** with your HubSpot OAuth2 API credentials in Workflow².
7. If you are using the [HubSpot Trigger](/workflow/integrations/trigger-nodes/workflow-nodes-base.hubSpotTrigger/) node, copy the **App ID** along with the information in the previous step.
8. Copy your OAuth Callback URL from the 'Create New Credentials' screen in Doc² and paste in the **Redirect URL** section.
9. In the Scopes section, select the following scopes in the **Find a scope** search box:
    * Trigger node:
        * oauth
        * crm.objects.contacts (read),
        * crm.schemas.contacts (read),
        * crm.objects.companies (read),
        * crm.schemas.companies (read),
        * crm.objects.deals (read),
        * crm.schemas.deals (read),
    * Regular node:
        * oauth
        * crm.schemas.deals (read),
        * crm.objects.owners (read),
        * crm.objects.contacts (write),
        * crm.objects.companies (write),
        * crm.objects.companies (read),
        * crm.objects.deals (read),
        * crm.schemas.contacts (read),
        * crm.objects.deals (write),
        * crm.objects.contacts (read),
        * crm.schemas.companies (read),
        * forms,
        * tickets,
11. Click on the **Save** button to save your settings in HubSpot.
12. Back in Doc², click on the circle button in the OAuth section to connect your HubSpot account to Workflow².
13. Click the **Save** button to save your credentials.


## Using API key

1. Access your HubSpot dashboard.
2. Click on the gear icon on the top right.
3. Click on **Integrations** and then **API key**.
4. Click on the **Create key** button.
5. Use the key with HubSpot node credentials in Workflow².


## Using APP Token

1. Follow the instructions in the [Private Apps Documentation](https://developers.hubspot.com/docs/api/private-apps) to get your access token.
2. Set the access token as the key in your HubSpot credentials in Workflow².


## Using Developer API Key (for HubSpot Trigger node)

1. Access your [HubSpot Developer Home](https://developers.hubspot.com/).
2. Click on **Apps** in the top bar.
3. Click on the **Get HubSpot API key** button.
4. Click on the **Show key** button.
5. Use the displayed Developer API key with your HubSpot Trigger node credentials in Workflow².
