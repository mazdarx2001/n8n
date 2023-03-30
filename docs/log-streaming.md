---
description: Stream events from n8n to your logging tools.
---

# Log streaming

!!! info "Feature availability"
	Log streaming is available on Enterprise Self-hosted and custom Cloud plans.


Log streaming allows you to send events from n8n to your own logging tools. This allows you to manage your n8n monitoring in your own alerting and logging processes.

## Set up log streaming

To use log streaming, you have to add a streaming destination.

1. Navigate to **Settings** > **Log Streaming**.
2. Select **Add new destination**.
3. Choose your destination type. n8n opens the **New Event Destination** modal.
4. In the **New Event Destination** modal, enter the configuration information for your event destination. These depend on the type of destination you're using.
5. Select **Events** to choose which events to stream.
6. Select **Save**.

!!! note "Self-hosted users"
	If you self-host n8n, you can configure additional log streaming behavior using [Environment variables](/hosting/environment-variables/environment-variables/#log-streaming).

## Events

The following events are available. You can choose which events to stream in **Settings** > **Log Streaming** > **Events**.

* Workflow
	* Started
	* Success
	* Failed
* Node executions
	* Started
	* Finished
* Audit
	* User signed up
	* User updated
	* User deleted
	* User invited
	* User invitation accepted
	* User reinvited
	* User email failed
	* User reset requested
	* User reset
	* User credentials created
	* User credentials shared
	* User API created
	* User API deleted
	* Package installed
	* Package updated
	* Package deleted
	* Workflow created
	* Workflow deleted
	* Workflow updated

## Destinations

n8n supports three destination types:

* A syslog server
* A generic webhook
* A Sentry client
