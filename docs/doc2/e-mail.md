---
title: "E-Mail"
date: "2021-10-22"
description: DOC² Email Import. If you want to import documents from your email inbox automatically, here are the steps you need to take.
tags:
  - E-Mail
  - Import
  - DOC²
---

### If you want to import documents from a specific email folder, here are the steps you need to take:

Your email folder could look like this.

![](/_images/doc2/AllImportOptions_Email_Folder.png)


Go to SETTINGS in the top bar and click on "Import".

![](/_images/doc2/AllImportOptions_Email_1.png)

As you can see, there is no email account setup for the import yet.

![](/_images/doc2/AllImportOptions_Email_2.png)

Click on the `OFF` button to open the Email import settings.

The boxes for E-Mail and Password as well as the API Key might get automatically filled in with your login information for DOC², depending on your browser settings. Please empty the fields before continuing to enter the needed information for the E-Mail Import.

What you need to do is enter the protocol (IMAP or POP3), the encryption (SSL or TSL), server-name, port, a username (e.g. "incoming invoices") as well as the email address and password from which the documents are going to be imported from.

This example is for a google email account:

!!! note "Important due to changes made by Google"
		You now need to set up 2-Factor Authentication and create an App-Password which you have to use here to make sure that the E-Mail import will work.

![](/_images/doc2/AllImportOptions_Email_3.png)

After you have entered all required fields of your respective provider, save the data.

![](/_images/doc2/AllImportOptions_Email_4.png)

You can test the login by pressing the `TEST LOGIN` button. If all data is correct you will get the following feedback.

![](/_images/doc2/AllImportOptions_Email_5.png)

After you click the `IMPORT` button, the documents will be fetched from the mailbox and you will be taken directly to the Dashboard.

![](/_images/doc2/AllImportOptions_Email_6.png)


If you have made the right decision to also use our [Workflow² APP](https://docs.polydocs.io/workflow/), you will find the corresponding workflows [here](https://docs.polydocs.io/example/gmail-import/) to automatically import your documents from your e-mail inbox to DOC².