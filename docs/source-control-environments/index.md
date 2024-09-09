---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: Source control and environments
description: Overview of source control and environments in n8n
contentType: overview
hide:
  - toc
---

# Source control and environments

--8<-- "_snippets/source-control-environments/feature-availability.md"

n8n uses Git-based source control to support environments. Linking your n8n instances to a Git repository lets you create multiple n8n environments, backed by Git branches.

In this section:

* [Understand](/source-control-environments/understand/):
	* [Environments in n8n](/source-control-environments/understand/environments/): The purpose of environments, and how they work in n8n.
	* [Git and n8n](/source-control-environments/understand/git/): How n8n uses Git. 
	* [Branch patterns](/source-control-environments/understand/patterns/): The possible relationships between n8n instances and Git branches.
* [Set up source control for environments](/source-control-environments/setup/): How to connect your n8n instance to Git.
* [Using](/source-control-environments/using/):
	* [Push and pull](/source-control-environments/using/push-pull/): Send work to Git, and fetch work from Git to your instance.
	* [Copy work between environments](/source-control-environments/using/copy-work/): How to copy work between different n8n instances.
	* [Manage variables](/source-control-environments/using/manage-variables/): Manage variable values using the n8n API and source control.
* [Tutorial: Create environments with source control](/source-control-environments/create-environments/): An end-to-end tutorial, setting up environments using n8n's recommended configurations.

Related sections:

* [Variables](/code/variables/): reusable values.
* [External secrets](/external-secrets/): manage credentials with an external secrets vault.
