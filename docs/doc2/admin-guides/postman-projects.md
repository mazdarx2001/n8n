---
title: "DOC² - Postman Guides"
description: This guide will help you learn how to make http requests via Postman to your DOC² Organization.
date: "2022-10-20"
tags:
  - DOC²
  - Postman
  - Guide
  - Setup
  - HTTP request
  - Admin
---


# Postman for DOC²


This guide will show you how to make HTTP requests to your DOC² organization via Postman. It is easy to use and very useful for organization administrators.


## Setup


First, [download Postman](https://www.postman.com/downloads/) to your system and sign in/register.

Now follow this step-by-step guide to learn how HTTP requests work in Postman.


## Authorization

### In Postman

Before you can create your HTTP requests, you need to enter your API key from DOC² to authorize them.

**1.** Click on the `Authorization` tab und choose `API Key` as authorization type.

![Picture](/_images/doc2/admin_guides_authorization_API Key.png){ loading=lazy }

**2.**  Fill in the values. Enter "x-api-key" in the `Key` field and your API Key as value (found in DOC² Settings menu **Integration**) Select the Add to `Header`.

It should look like this:

![Picture](/_images/doc2/admin_guides_authorize_finish.png){ loading=lazy }

### On <a href="https://api.polydocs.io">api.polydocs.io</a>

**1.** Click on **Authorize** in the upper right corner

![Picture](/_images/doc2/admin_guides_doc2-api-authorize.png){ loading=lazy }

**2.** Enter your API Key and confirm by clicking `Authorize`

![Picture](/_images/doc2/admin_guides_doc2-api-authorize_key.png){ loading=lazy }


## Create a new Workspace in Postman

**1.**  Click on Workspaces and create a new workspace (you can name it whatever you want).<br>

![Picture](/_images/doc2/admin_guides_postman_guide_workspace_1.png){ loading=lazy }

**2.**  You have to select the visibility which determines who can access this workspace.

![Picture](/_images/doc2/admin_guides_postman_guide_create-workspace-visibility.png){ loading=lazy }

**3.**  After making your selection and clicking `Create Workspace` select Collections on the left side of the application and create a new collection for your HTTP requests by clicking `+`.

![Picture](/_images/doc2/admin_guides_postman_guide_new collection.png){ loading=lazy }

In this collection, you can add multiple HTTP requests. To do this, click on the 3 points of the collection and select `Add request`.

![Picture](/_images/doc2/admin_guides_add_request.png){ loading=lazy }


## "GET" Method example

The GET method is very useful to get information about users, sub-organizations, processed documents and much more.

**1.**  Choose the GET method in your HTTP request.<br>
**2.**  Authorize yourself as described [above](/doc2/admin-guides/postman-projects/#authorization).<br>
**3.**  Open <a href="https://api.polydocs.io">api.polydocs.io</a> and add the path of the function behind the polydocs URL. For example:

![Picture](/_images/doc2/admin_guide_get_api.png){ loading=lazy }



        https://api.polydocs.io/users/get_users


**4.**  Now paste this link in the text box next to the GET method in Postman.

Click `Send` and you should receive all the information about every user in your organization.


## "POST" Method examples

The POST method is usually used to create users or organizations, for example. This method inserts information into the database.

### Create User

**1.**  Select the POST Method.<br>
**2.**  Authorize yourself as described [above](/doc2/admin-guides/postman-projects/#authorization).<br>
**3.**  Open <a href="https://api.polydocs.io">api.polydocs.io</a> and add the path of the function behind the polydocs URL. In this case:

![Picture](/_images/doc2/admin_guides_post_api.png){ loading=lazy }
    


    https://api.polydocs.io/users/create


**4.**  Now paste this link into the text box next to the POST method in Postman.<br>
**5.**  Select the `Body` tab in your HTTP request and enter the keys and the values ​​for each credential that has a red asterisk next to its name.

When you're done, it should look like this:

![Picture](/_images/doc2/admin_guide_post_body.png){ loading=lazy }

If you want to create an admin account, set the `is_admin` value to **true**.

Finally, click `Send` and you can see all the credentials you set in the response below. This means the user has been created.

![Picture](/_images/doc2/admin_guides_post_response.png){ loading=lazy }


### Upload document

You can also use the POST method to upload a document to DOC².

**1.**  Select the POST Method.<br>
**2.**  Authorize yourself as described [above](/doc2/admin-guides/postman-projects/#authorization).<br>
**3.**  Open <a href="https://api.polydocs.io">api.polydocs.io</a> and add the path of the function behind the polydocs URL. In this case:

![Picture](/_images/doc2/admin_guides_post_document-process.png){ loading=lazy }
    


    https://api.polydocs.io/document/process


**4.**  Now paste this link into the text box next to the POST method in Postman.<br>
**5.**  Select the `Body` tab in your HTTP request and choose `form-data`
![Picture](/_images/doc2/admin_guides_post_document-process_body-form-data-file.png){ loading=lazy } 
![Picture](/_images/doc2/admin_guides_post_document-process_key-value-send.png){ loading=lazy }
**6.**  Enter **file** into the `KEY` field where you will find the hidden File dropdown. Select `File` and move to the `VALUE` field where you are able to select your file by clicking `Select Files`. 
**7.** When you click `Send`, you should see "success": true in the response.

It should look like this:

![Picture](/_images/doc2/admin_guides_upload_body.png){ loading=lazy }


## "DELETE" Method example

The DELETE method is used to delete, for example, users, organizations and so on.

**1.**  Select the DELETE Method.<br>
**2.**  Authorize yourself as described [above](/doc2/admin-guides/postman-projects/#authorization).<br>
**3.**  Open <a href="https://api.polydocs.io">api.polydocs.io</a> and add the path of the function behind the polydocs URL. For example:

![Picture](/_images/doc2/admin_guides_delete_api.png){ loading=lazy }



    https://api.polydocs.io/users/delete/{user_id}



**4.**  Now paste this link in the text box next to the DELETE method in Postman.<br>
**5.**  Replace the {user_id} at the end of the URL with the actual user ID you want to delete. (You can get the user_id using the GET method).<br>
**6.**  If you included the user_id in the URL, you don't need to add a body key and value for it.
**7.**  When you click `Send`, you should see "success": true in the response.

It should look like this:

![Picture](/_images/doc2/admin_guides_delete_body.png){ loading=lazy }


## "PUT" Method example

The PUT method is mainly used to update user or organization data. It is very easy to understand and use.

**1.**  Select the PUT Method.<br>
**2.**  Authorize yourself as described [above](/doc2/admin-guides/postman-projects/#authorization).<br>
**3.**  Open <a href="https://api.polydocs.io">api.polydocs.io</a> and add the path of the function behind the polydocs URL. For example:

![Picture](/_images/doc2/admin_guides_put_api.png){ loading=lazy }


    
    https://api.polydocs.io/users/update/{user_id}



**4.**  Now paste this link in the text box next to the PUT method in Postman.<br>
**5.**  Replace the {user_id} at the end of the URL with the actual user ID you want to delete. (You can get the user_id using the GET method).

Suppose you want to change the email address of a user in your organization.

**1.**  In the body, enter "email" as the key and the new email address as the value.<br>
**2.**  Then just press `Send` and you should see "success" in the response.


If you'd like to have this all more visualized and interactive, you can download the Postman project <a href="/example/downloadables/doc2app.postman_collection.json" download>here</a> to try it all out.
Just click the Import button and select this file to get started right away.

![Picture](/_images/doc2/admin_guides_import_json.png){ loading=lazy }