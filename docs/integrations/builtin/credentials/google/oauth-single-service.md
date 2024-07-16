---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: Google OAuth2 single service
description: Documentation for single service OAuth2 Google credentials. Use these credentials to authenticate Google in n8n, a workflow automation platform.
contentType: integration
priority: critical
---

# Google: OAuth2 single service

This document contains instructions for creating a Google credential for a single service. They're also available as a [video](#video).

--8<-- "_snippets/integrations/managed-google-oauth.md"

## Prerequisites

* [Google Cloud](https://cloud.google.com/){:targe=_blank .external-link} account
* [Google Cloud Platform project](https://developers.google.com/workspace/marketplace/create-gcp-project){:targe=_blank .external-link}
* If you haven't used OAuth in your Google Cloud project before, you need to [configure the OAuth consent screen](https://developers.google.com/workspace/guides/configure-oauth-consent){:target=_blank .external-link}.
* If using Google Perspective: [Request API Access](https://developers.perspectiveapi.com/s/docs-get-started){:targe=_blank .external-link}
* If using Google Ads: [Developer Token](https://developers.google.com/google-ads/api/docs/first-call/dev-token){:targe=_blank .external-link}


## Set up OAuth

### Create a new credential in n8n

1. Follow the steps to [Create a credential](/credentials/add-edit-credentials/).

    /// note | Generic and specific credentials
    If you create a credential by selecting **Create new** in the credentials dropdown in a node, n8n automatically creates the correct credential type for that node. If you select **Credentials > New**, you must browse for the credential type:

	* To connect with a specific service, using resources and operations supported by n8n, choose that service. For example, to create a credential for use in the Gmail node, search for `Gmail`.
	* To create a credential for a [custom API call](/integrations/custom-operations/), select **Google OAuth2 API**. This allows you to create a generic credential, then set its scopes.
    ///

2. Note the **OAuth Redirect URL** from the node credential modal. You'll need this in the next section.

	??? Details "View screenshot"
		![OAuth Callback URL](/_images/integrations/builtin/credentials/google/oauth_callback.png)


### Set up OAuth in Google Cloud

1. Go to [Google Cloud Console | APIs and services](https://console.cloud.google.com/apis/credentials){:target=_blank .external-link} and make sure you're in the project you want to use.

	??? Details "View screenshot"
		![Google project dropdown](/_images/integrations/builtin/credentials/google/check-google-project.png)

2. **Optional:** If you haven't used OAuth in your Google Cloud project before, you need to [configure the OAuth consent screen](https://developers.google.com/workspace/guides/configure-oauth-consent){:target=_blank .external-link}. Expand the detailed steps below for more guidance.

	??? Details "View detailed steps"
		1. Select **OAuth consent screen**.
		2. For **User Type**, select **Internal** for user access within your organization's Google workspace or **External** for any user with a Google account.
		3. Select **Create**.
		4. Enter the essential information: **App name**, **User support email**, and the **Email addresses** field in **Developer contact information**.
		5. Add an authorized domain: select **+ ADD DOMAIN**. Enter `n8n.cloud` if using n8n's Cloud service, or the domain of your n8n instance if you're self-hosting.
		6. Select **SAVE AND CONTINUE** to go to the **Scopes** page.
		7. You don't need to set any scopes. Select **SAVE AND CONTINUE** again to go to the **Summary** page.
		8. On the **Summary** page, review the information, then select **BACK TO DASHBOARD**.

3. Select **+ CREATE CREDENTIALS > OAuth client ID**.

	??? Details "View screenshot"   
		![Create credentials](/_images/integrations/builtin/credentials/google/create-credentials.png)

4. In the **Application type** dropdown, select **Web application**. Google automatically generates a name.

	??? Details "View screenshot"   
		![Web application](/_images/integrations/builtin/credentials/google/application-web-application.png)

5. Under **Authorized redirect URIs**, select **+ ADD URI**. Paste in the OAuth redirect URL from n8n.

	??? Details "View screenshot"  
		![OAuth Callback URL](/_images/integrations/builtin/credentials/google/oauth_callback.png) 
		![Add URI](/_images/integrations/builtin/credentials/google/add-uri.png)

6. Select **CREATE**.
7. Enable each Google service API that you want to use:

	1. If using Google Perspective or Google Ads: [Request API Access for Perspective](https://developers.perspectiveapi.com/s/docs-get-started){:target=_blank .external-link} or a [Developer Token for Ads](https://developers.google.com/google-ads/api/docs/first-call/dev-token){:target=_blank .external-link}.  
	--8<-- "_snippets/integrations/builtin/credentials/google/enable-apis.md"

### Create and test your connection

In n8n:

1. Enter your new **Client ID** and **Client Secret** from Google Cloud Console in the credentials modal.
2. Select **Sign in with Google** to complete your Google authentication.
3. **Save** your new credentials.

## Video

<div class="video-container">
<iframe width="840" height="472.5" src="https://www.youtube.com/embed/gZ6N2H3_vys" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

## Troubleshooting

### Google hasn't verified this app

--8<-- "_snippets/integrations/builtin/credentials/google/unverified-app.md"

### Google Cloud app becoming unauthorized

--8<-- "_snippets/integrations/builtin/credentials/google/app-becoming-unauthorized.md"

