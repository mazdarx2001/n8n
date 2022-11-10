---
title: SMTP
description: SMTP plugin can connect Insight² applications to SMTP servers for sending emails.
tags:
  - Insight²
  - Data Sources
  - SMTP
---

# SMTP

SMTP plugin can connect Insight² applications to **SMTP servers** for sending emails.

## Connection

A SMTP server can be connected with the following credentails:
- **Host**
- **Port**
- **User**
- **Password**

:fontawesome-solid-circle-info:{ style="color: #0F17E4" }
You can also test your connection before saving the configuration by clicking on `Test Connection` button.




![Insight² - Data source - WF²](/_images/insight2/datasource-reference/smtp/connect.png)



## Querying SMTP

Go to the query manager at the bottom panel of the editor and click on the `+` button on the left to create a new query. Select `SMTP` from the datasource dropdown.

To create a query for sending email, you will need to provide the following properties:
  - **From** `required` : Email address of the sender
  - **From Name** : Name of the sender
  - **To** `required` : Recipient's email address
  - **Subject** : Subject of the email



![Insight² - Data source - WF²](/_images/insight2/datasource-reference/smtp/query1.png)



  - **Body** : You can enter the body text either in the form of `raw text` or `html` in their respective fields.
  - **Attachments** : Attachments can be added to a SMTP query by referencing the file from the `File Picker` component in the attachments field.

  For example, you can set the `Attachments` field value to `{{ components.filepicker1.file }}` or you can pass an array of `{{ name: 'filename.jpg', dataURL: '......' }}` object to accomplish this.



![Insight² - Data source - WF²](/_images/insight2/datasource-reference/smtp/query2.png)


