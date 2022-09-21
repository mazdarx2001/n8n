---
title: DynamoDB
description: Insight² can connect to DynamoDB to read and write data. Learn more about it here and improve your workflows.
tags:
  - Insight²
  - Data Sources
  - DynamoDB
---

# DynamoDB

Insight² can connect to DynamoDB to read and write data.

## Connection

To add a new DynamoDB, click on the `+` button on data sources panel at the left-bottom corner of the app editor. Select DynamoDB from the modal that pops up.

Insight² requires the following to connect to your DynamoDB.

- **Region**
- **Access key**
- **Secret key**

It is recommended to create a new IAM user for the database so that you can control the access levels of Insight².

<img src="/_images/insight2/datasource-reference/dynamo-connect.png" alt="Insight² - Dynamo connection" height="250"/>

Click on `Test Connection` button to verify if the credentials are correct and that the database is accessible to Insight² server. Click on `Save` button to save the data source.

## Querying DynamoDB

Click on `+` button of the query manager at the bottom panel of the editor and select the database added in the previous step as the data source. Select the operation that you want to perform and click  `Save`  to save the query.

<img src="/_images/insight2/datasource-reference/dynamo-query.png" alt="Insight² - Dynamo query" height="250"/>

Click on the `run` button to run the query.<br>  
:fontawesome-solid-triangle-exclamation:{ style="color: #EE0F0F" } 
**NOTE**: Query should be saved before running.
:fontawesome-solid-triangle-exclamation:{ style="color: #EE0F0F" }

:fontawesome-solid-circle-info:{ style="color: #0F17E4" }
Query results can be transformed using transformations. Read our transformations documentation to see how: [link](/insight2/tutorial/transformations/)

