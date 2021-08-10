---
permalink: /credentials/nocoDb
description: Learn to configure credentials for the NocoDB node in n8n
---

# NocoDB

You can use these credentials to authenticate the following nodes:
- [NocoDB](../../nodes-library/nodes/nocoDb/README.md)

## Prerequisites

* Install [NocoDB](https://www.nocodb.com/)
* Enable [API Access](https://docs.nocodb.com/setup-and-usages/apis-access)

## Using Auth Token

From n8n:

1. Enter a descriptive ***Credentials Name***.
2. In the ***Credentials Data*** section enter the following:
    * ***API Token***: The authentication token for your NocoDB project, obtained when enabling API access (above).
    * ***Host***: The host of your NocoDB instance, for example `http://localhost:8080`.
3. Click **Create** to save your new credentials.