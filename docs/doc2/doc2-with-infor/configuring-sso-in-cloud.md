---
title: "Configuring SSO in Infor Cloud"
date: "2021-10-14"
description: This is a step by step guide how to configure SSO in Infor Cloud. Starting with the prerequisites, getting access to the cloud and checking it to add a new service provider.
tags:
  - Infor
  - SSO
  - Cloud
  - new service provider
---

# Configuring SSO in Infor Cloud

## Step by step guide

### **Prerequisites**

<table><tbody><tr><td><strong>Required Information</strong></td><td><strong>Description</strong></td></tr><tr><td>Login Details to Cloud</td><td>Credentials are mandatory for accessing the Infor Cloud environment.<br>The user should have the roles "Infor-SystemAdministrator" and "UserAdmin".</td></tr><tr><td>Config Admin Details (DOC²)</td><td>You should have received an email from Polydocs GmbH with the login details for the DOC² SSO Settings page.<br><br>You will need a login and password.<br></td></tr><tr><td>Certificate</td><td>You can download the certificate in DOC² under SSO Service Provider Settings.</td></tr></tbody></table>

**1\. Get access to the Cloud and check your access**

The URL starts with [https://mingle-portal.eu1.inforcloudsuite.com/<TENANT\_NAME](https://mingle-portal.eu1.inforcloudsuite.com/)\> followed by your personal extension.

![](/_images/doc2/infor-signin-1024x520.png){ loading=lazy }

a) Choose the option "Cloud Identities" and fill in your login details.

![](/_images/doc2/LogIn-infor-1024x640.png){ loading=lazy }

b) After you have logged in, you will have access to the Infor Cloud. You will be taken to this page, but on the burger menu you will find access to all the applications.

![](/_images/doc2/Welcome-to-infor-Ming.le_-1024x585.png){ loading=lazy }

![](/_images/doc2/infor_Burger-Menu-1024x586.png){ loading=lazy }

**2\. Open "User Management" to add a new Service Provider**

On the right hand side of the bar menu, you will find the user menu and that is where you can access user management

![](/_images/doc2/infor_User-Management-1024x548.png){ loading=lazy }

a) Then, in the left hand side menu, you need to select  the option **Security Administration** and **Service Provider**.

![](/_images/doc2/infor_Service-Provider-1024x523.png){ loading=lazy }

b. You will see this window with the Service Providers.

![](/_images/doc2/infor_Service-Provider_2-1-1024x479.png){ loading=lazy }

c. Now click on the “+” sign and add DOC² as Service Provider. (View step 4)

![](/_images/doc2/infor6.png){ loading=lazy }

**3\. Access the SSO SERVICE PROVIDER SETTINGS in DOC²**

a) Log in using the URL [https://app.polydocs.io/](https://app.polydocs.io/) with the login details you received from us.

b) Go to SETTINGS (on top bar) and choose "SSO Settings" down at the bottom of the list.

Here you will find all the information you need for the following steps.

c) Download the certificate

![](/_images/doc2/DOC2_SSO-Service-Provider-Settings-1024x640.png){ loading=lazy }

**4\. Filling in the Service Provider details with the help of SSO Service Provider Settings in DOC²**

![](/_images/doc2/infor_Service-Provider_3-1024x891.png)

<table><tbody><tr><td><strong>Field</strong></td><td><strong>Value</strong></td></tr><tr><td><strong>Application Type</strong></td><td>DEFAULT_SAML</td></tr><tr><td><strong>Display Name</strong></td><td>DOC²</td></tr><tr><td><strong>Entity ID</strong></td><td>See Entity ID under SSO SERVICE SETTINGS</td></tr><tr><td><strong>SSO Endpoint</strong></td><td>Copy the SSO URL from SSO SERVICE SETTINGS and paste it in the <strong>SSO Endpoint </strong>field.</td></tr><tr><td><strong>SLO Endpoint</strong></td><td>Copy SLO URL from SSO SERVICE SETTINGS and paste it in the <strong>SLO Endpoint </strong>field.</td></tr><tr><td><strong>Signing Certificate</strong></td><td>Upload the appropriate .cer file you have downloaded in step 3c) from SSO SERVICE SETTINGS</td></tr><tr><td><strong>Name ID Format and Mapping</strong></td><td>emailaddress</td></tr></tbody></table>

![](/_images/doc2/infor_Service-Provider_completed-956x1024.png)

a) When you have filled out everything remember to save it with the disk icon above Application Type

b) Then, enter the details of the service provider DOC² again.

c) Click on "VIEW" underneath Identity Provider Information.

![](/_images/doc2/infor_Identity-Provider-Information-copy-1024x559.png){ loading=lazy }

![](/_images/doc2/infor_Identity-Provider-Information-806x1024.png){ loading=lazy }

d) Export the **SAML METADATA.**

The file looks like this: ServiceProviderSAMLMetadata\_10\_20\_2021.xml

**5\. Import the SAML METADATA in the SSO Settings.**

Go to IDENTITY SERVICE PROVIDER SETTINGS, enter your Tenant ID (e.g. FELLOWCONSULTING\_DEV and underneath that line you will see Upload file and the IMPORT Button, this is where you need to upload the previously exported SAML METADATA file.

a) Click on IMPORT and then choose the METADATA file that you have already downloaded from the SSO SERVICE PROVIDER SETTINGS

b) Click on CONFIGURE

![](/_images/doc2/DOC2_identity-service-provider-settings_completed-1024x316.png){ loading=lazy }

This part is successfully completed when you see the following pop-up.

![](/_images/doc2/DOC2_File-successfully-saved.png){ loading=lazy }

**6\. Adding a new Application in Infor Ming.le**

a) Go to Admin Settings

![](/_images/doc2/infor_Admin-Settings_Manage-Applications-1024x528.png){ loading=lazy }

b) Click on ADD APPLICATION in the top right corner

![](/_images/doc2/infor_Add-Application.png){ loading=lazy }

c) Fill out all the required fields, like in the image below, but with your own SSO Url. Don't forget to choose an icon and click on SAVE

![](/_images/doc2/infor_Add-New-Application.png){ loading=lazy }

**The final step:**

- Log out of DOC²
- Go back to the burger menu in Infor and select the icon you just created
- You should then be at the dashboard of DOC²

![](/_images/doc2/Sign-in-over-SSO-1024x640.png){ loading=lazy }
