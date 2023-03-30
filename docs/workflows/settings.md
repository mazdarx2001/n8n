---
description: Manage settings for an individual workflow.
---

# Workflow settings

You can customize workflow behavior for individual workflows using workflow settings.

To open the settings:

1. Open your workflow.
2. Select the **Options** <span class="inline-image">![Options menu](/_images/common-icons/three-dot-options-menu.png)</span> menu.
3. Select **Settings**. n8n opens the ** Workflow settings** modal.


The following settings are available:

* **Error Workflow**: select a workflow to trigger if the current workflow fails. See [Error workflows](/flow-logic/error-handling/error-workflows/) for more details.
* **This workflow can be called by**: choose whether other workflow can call this workflow. Requires [Workflow sharing](/workflows/sharing/).
* **Timezone**: sets the timezone for the workflow to use. The default timezone is EDT (New York). The timezone setting is  important for the Schedule trigger node.
* **Save failed production executions**: whether n8n should save failed executions for active workflows.
* **Save successful production executions**: whether n8n should save successful executions for active workflows.
* **Save manual executions**: whether n8n should save executions for workflows started by the user in the editor.
* **Save execution progress**: whether n8n should save execution data for each node. If set to **Yes**, the workflow resumes from where it stopped in case of an error. This might increase latency.
* **Timeout Workflow**: toggle to enable setting a duration after which n8n should cancel the current workflow execution.
	* **Timeout After**: Set the time in hours, minutes, and seconds after which the workflow should timeout. For n8n Cloud users n8n enforces a maximum available timeout for each plan.
