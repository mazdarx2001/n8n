---
title: MS SQL Server / Azure SQL databases
description: 
tags:
  - Insight²
  - Data Sources
---

# MS SQL Server / Azure SQL databases


Insight² can connect to MS SQL Server & Azure SQL databases to read and write data.

## Connection

Please make sure the host/ip of the database is accessible from your VPC if you have self-hosted Insight². If you are using Insight² cloud, please whitelist our IP.

To add new MS SQL Server / Azure SQL database, click on the **Add or edit datasources** icon on the left sidebar of the app editor and click on `+ add data source` button. Select **SQL Server** from the modul that pops up.

Insight² requires the following to connect to your PostgreSQL database.

- **Host**
- **Port**
- **Username**
- **Password**
- **Azure** - Select this option if you are using Azure SQL databases.

It is recommended to create a new database user so that you can control the access levels of Insight².

Click on `Test Connection` button to verify if the credentials are correct and that the database is accessible to Insight² server. Click on `Save` button to save the data source.

<img src="/_images/insight2/datasource-reference/mssql/connect.gif" alt="Insight² - Redis connection" height="420"/>


## Querying SQL Server / Azure SQL databases
Click on `+` button of the query manager at the bottom panel of the editor and select the database added in the previous step as the data source.

Click on the `run` button to run the query.<br> :fontawesome-solid-triangle-exclamation:{ style="color: #EE0F0F" } **NOTE**: Query should be saved before running.

<img src="/_images/insight2/datasource-reference/mssql/query.gif" alt="Insight² - Redis connection" height="420"/>


:fontawesome-solid-circle-info:{ style="color: #0F17E4" } **TIP**:
Query results can be transformed using transformations. Read our transformations documentation to see how: [link](/insight2/tutorial/transformations/)

