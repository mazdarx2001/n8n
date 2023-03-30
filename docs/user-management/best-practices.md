---
description: User management best practices.
---

# Best practices for user management

This page contains advice on best practices relating to user management in n8n.

## All platforms

* We recommend that owners create a member-level account for themselves. Owners can see all workflows, but there is no way to see who created a particular workflow, so there is a risk of overriding other people's work if you build and edit workflows as an owner.
* Users must be careful not to edit the same workflow simultaneously. It's possible to do it, but the users will overwrite each other's changes.
* To move workflows between accounts, export the workflow as JSON, then import it to the new account. Note that this action loses the workflow history.
* Webhook paths must be unique across the entire instance. This means each webhook path must be unique for all workflows and all users. By default, n8n generates a long random value for the webhook path, but users can edit this to their own custom path. If two users set the same path value:
    * The path works for the first workflow that is run or activated.
    * Other workflows will error if they try to run with the same path.

## Self-hosted

* If you run n8n behind a reverse proxy, set the following environment variables so that emails are generated with the correct URL:
	* `N8N_HOST`
	* `N8N_PORT`
	* `N8N_PROTOCOL`
	* `N8N_EDITOR_BASE_URL`  
  More information on these variables is available in [Environment variables](/hosting/environment-variables/environment-variables/).
* You can't use n8n's user management with basic auth. If your n8n instance currently uses basic auth to authenticate the user, you must remove this before setting up user management.
