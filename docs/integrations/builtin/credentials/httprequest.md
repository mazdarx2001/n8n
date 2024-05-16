---
title: HTTP Request credentials
description: Documentation for HTTP Request credentials. Use these credentials to authenticate HTTP Request in n8n, a workflow automation platform.
contentType: integration
---

# HTTP Request credentials

You can use these credentials to authenticate the following nodes:

- [HTTP Request](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/)

## Prerequisites

You must use the authentication method required by the app or service you want to query.

### Predefined credential types

n8n recommends using this option whenever there's a credential type available for the service you want to connect to. It offers an easier way to set up and manage credentials, compared to configuring generic credentials.

You can use [Predefined credential types](/integrations/custom-operations/#predefined-credential-types) to perform custom operations with some APIs where n8n has a node for the platform. For example, n8n has an Asana node, and supports using your Asana credentials in the HTTP Request node. Refer to [Custom operations](/integrations/custom-operations/) for more information.

### Using a predefined credential type

--8<-- "_snippets/integrations/predefined-credential-type-how-to.md"

Refer to [Custom API operations](/integrations/custom-operations/) for more information.

## Generic authentication

The following generic authentication methods are available:

* Basic Auth
* Custom Auth
* Digest Auth
* Header Auth
* OAuth1 API
* OAuth2 API
* Query Auth

You can learn more about HTTP authentication [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/Authentication#see_also){:target=_blank .external-link}.

### Using Basic Auth or Digest Auth

1. Update the credential name.
2. Enter the **Username** and **Password** for the app or service your HTTP Request is targeting. 
3. Select **Save** to save your credentials.

### Using Header Auth

1. Update the credential name.
2. Enter the header **Name** and **Value** required for the app or service your HTTP Request is targeting. Read more about [HTTP headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers#authentication){:target=_blank .external-link}.
3. Select **Save** to save your credentials.

### Using OAuth1

1. Update the credential name.
2. Enter the following authentication details:
    * **Authorization URL**
    * **Access Token URL**
    * **Consumer Key**
    * **Consumer Secret**
    * **Request Token URL**
    * **Signature Method**
3. Select **Save** to save your credentials.

Read more about [OAuth1](https://oauth.net/1/){:target=_blank .external-link}.

### Using OAuth2

1. Update the credential name.
2. Enter the following authentication details:
    * **Authorization URL**
    * **Access Token URL**
    * **Client ID**
    * **Client Secret**
    * **Scope**
    * **Auth URI Query Parameters**
    * **Authentication**
3. Select **Save** to save your credentials.

Read more about [OAuth2](https://oauth.net/2/){:target=_blank .external-link}.

### Using Custom Auth

The **Generic Auth Type** > **Custom Auth** option expects JSON data to define your credential. You can define credentials using headers, qs, body, or a combination of these within a parent `json` key. See the examples below to get started.

#### Sending two headers
```
{
	"json": {
		"headers": {
			"X-AUTH-USERNAME": "username",
			"X-AUTH-PASSWORD": "password"
		}
	}
}
```

#### Body
```
{
	"json": {
		 "body" : {
			"user": "username",
			"pass": "password"
		}
	}
}
```

#### Query string
```
{
	"json": {
		"qs": { 
			"appid": "123456",
			"apikey": "my-api-key"
		}
	}
}
```

#### Sending header and query string
```
{
	"json": {
		"headers": {
			"api-version": "202404"
		},
		"qs": {
			"apikey": "my-api-key"
		}
	}
}
```

## Provide an SSL certificate

You can send an SSL certificate with your HTTP request. You can use this alongside other credential types.

1. In the node **Settings** <span class="inline-image">![Settings icon](/_images/common-icons/settings.png){.off-glb}</span>, enable **SSL Certificates**.
1. On the **Parameters** tab, add the SSL credential to **Credential for SSL Certificates**.

