<!--
# How to use this template

1. Make a new branch. If working on an internal ticket, include it at the start of the name. For example, DOC-123-feature-summary.
2. Create a new file, or find the file you want to edit, in integrations/builtin/credentials/. If creating a new file, the name should be the integration name.
3. Copy the template into the file (don't copy this comment).
4. Placeholder text is in _italic_ or between <>. Make sure to replace it! 
5. Before publishing, delete any comments.

Use the style guide: https://github.com/n8n-io/n8n-docs/wiki
You can find more info on working with the docs project in the README: https://github.com/n8n-io/n8n-docs/blob/main/README.md

-->

<!--
Set the meta title and meta description in the frontmatter
-->

---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: _Name_ credentials
description: Documentation for the _Name_ credentials. Use these credentials to authenticate _Name_ in n8n, a workflow automation platform.
---

<!-- 
The title should be the name of the integration.
Match the brand name exactly. For example, GitHub NOT Github
-->
# _Name_ credentials

You can use these credentials to authenticate the following nodes:

* _List of apps_
* _That use these credentials_

<!--if this is a credential-only node, use this snippet instead-->
--8<-- "_snippets/integrations/builtin/credentials/cred-only-statement.md"

## Prerequisites

_Include info on services they need to sign up for_

## Supported authentication methods

## Related resources

<!-- add a link to the service's documentation. This should usually go direct to the API credential docs. Amend the link text if necessary. -->
Refer to [_Name_'s API documentation](){:target=_blank .external-link} for more information about authenticating with the service.


<!-- If this is a credential-only node, add a link to the node page on n8n's website. For example: https://n8n.io/integrations/gmail/ 
This is a credential-only node. Refer to [Custom API operations](/integrations/custom-operations/) to learn more. View [example workflows and related content](https://n8n.io/integrations/_Name_/){:target=_blank .external-link} on n8n's website. -->


## Using _Auth method_

To configure this credential, you'll need:

- _List of fields they'll need to fill out within n8n_
	
_Link to product's docs for this auth method._
	
_STOP AND THINK: does this node require a step by step? If authentication is easy to set up, or if this node isn't heavily used, consider leaving out the step by step to minimise maintenance._

_IF NEEDED: Include a step by step guide to how to set up a particular type of authentication. If multiple auth methods are available, create a section for each. For example, the Asana credentials have two sections: one for OAuth and one for access token (/integrations/builtin/credentials/asana/)_

<!-- IF OAUTH FOR CLOUD-HOSTED DOESN'T REQUIRE ANY SETUP, use the section below. Otherwise omit -->
--8<-- "_snippets/integrations/builtin/credentials/cloud-oauth-button.md"

If you need to configure OAuth2 from scratch or need more detail on what's happening in the OAuth web flow, refer to the instructions in the [_Name_ OAuth documentation](){:target=_blank .external-link} to set up OAuth.

<!-- 
Add any other sections here. 
You should include: quirks, pain points, complex topics that trip people up
-->
