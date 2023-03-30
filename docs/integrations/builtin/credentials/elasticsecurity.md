---
title: Elastic Security credentials
description: Documentation for Elastic Security credentials. Use these credentials to authenticate Elastic Security in n8n, a workflow automation platform.
---

# Elastic Security credentials

You can use these credentials to authenticate the following nodes:

- [Elastic Security](/integrations/builtin/app-nodes/n8n-nodes-base.elasticsecurity/)

## Prerequisites

- Create an [Elastic Security](https://www.elastic.co/security) account.
- [Deploy](https://www.elastic.co/guide/en/cloud/current/ec-create-deployment.html) an application.

## Using Basic Auth

**From Elastic Security**:

1. Navigate to your ***Dashboard*** > ***Deployments*** section and open the dashboard for the desired deployment.
2. From the ***Applications*** section, copy the endpoint of your application.

**From n8n**:

1. In the ***Credential Data*** section, enter your:
    * Username
    * Password
    * Base URL: The application endpoint obtained above.
2. Click ***Save*** to save your credentials.

