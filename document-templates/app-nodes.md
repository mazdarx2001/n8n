<!--
# How to use this template

1. Make a new branch. If working on an internal ticket, include it at the start of the name. For example, DOC-123-feature-summary.
2. Create a new file, or find the file you want to edit, in integrations/builtin/app-nodes/. If creating a new file, pay attention to the naming conventions: it should match the node name in the codex file. For example, in the Active Campaign node, the codex file (https://github.com/n8n-io/n8n/blob/master/packages/nodes-base/nodes/ActiveCampaign/ActiveCampaign.node.json) reads: `"node": "n8n-nodes-base.activeCampaign"`. So the app node file name is n8n-nodes-base.activeCampaign.
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
title: <node-name> node - n8n Documentation
description: Documentation for the <node-name> node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

<!-- 
The title should be the name of the integration 
Match the brand name exactly. For example, GitHub NOT Github
-->
# _Name_

_Briefly summarize the node. For example:_ 

_The Action Network node allows you to automate work in Action Network and integrate Action Network with other applications. n8n has built-in support for a wide range of Action Network features, which includes creating, updating, and deleting events, people, tags, and signatures._

_On this page, you'll find a list of operations the Action Network node supports, and links to more resources._

!!! note "Credentials"
    You can find authentication information for this node _here (link to credentials doc)_.

!!! note "Examples and templates"
	For usage examples and templates to help you get started, refer to n8n's [_Name's_ integrations](){:target=_blank .external-link} page.
	
## Operations

* _Bullet list_
* _Of available operations_.

## Related resources

<!-- add a link to the service's documentation. This should usually go direct to the API docs -->
Refer to [_Name's_ documentation](){:target=_blank .external-link} for more information about the service.

<!-- provide a link to the trigger node docs, if there is a trigger node for this service -->
n8n provides a trigger node for _Name_. You can find the trigger node docs [here]().
	
<!-- add a link to the node page on n8n's website. For example: https://n8n.io/integrations/356-gmail/ -->
View [example workflows and related content](){:target=_blank .external-link} on n8n's website.


<!-- 
Add any other sections here. 
You should include: quirks, pain points, complex topics that trip people up
You should not include: basic usage examples
-->
