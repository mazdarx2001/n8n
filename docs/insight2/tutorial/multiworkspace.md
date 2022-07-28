---
title: Multi-Workspace
description: 
tags:
  - Insight²
  - Workspace
---

# Multi-Workspace

User can create their own workspaces, user who created workspace will be having admin privileges for the workspace.


![Insight² - Google create project](/_images/insight2/multiworkspace/multi-workspace.gif)

## Hierarchy



![Insight² - Google create project](/_images/insight2/multiworkspace/Tooljet-workspace.png)



## Permissions

- The administrator can manage [users and groups](/insight2/tutorial/manage-users-groups/) of each workspace
- Applications and settings can not be shared between workspaces
- A user authorised to login to Insight² will not have access to all workspaces, Usesr should be invited or signed up to a workspace to log-in to it.

## Enabling Multi-Workspace

Set environment variable **DISABLE_MULTI_WORKSPACE** value to **false**  to enable the feature, and **true**  to disable it.

### When enabled

- When Multi-Workspace feature is enabled, user should login with username and password to log in to Tooljet.
- Administrator can configure authentication methods for their workspaces.
- If password login is enabled, switching to the workspace will happen without any other authorization since the user is already authorized with password login.
- User logged in to Toojet and trying to switch to a workspace where SSO is enabled and password login is disabled, will be redirected to workspace login page and enabled SSO options will be shown
- User can directly login to a workspace using workspace login URL, Administrator can view the URL **Manage SSO -> General Settings -> Login URL**.

### When disabled

- If Multi-Workspace is disabled, Create workspace feature won’t be available.
- No separate login page for workspace and SSO configured for the workspace will be reflected to the main login page/login.
