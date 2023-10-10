---
contentType: howto
description: How to handle execution errors.
---

# Error handling

When designing your flow logic, it's a good practice to consider potential errors, and set up methods to handle them gracefully. With an error workflow, you can control how n8n responds to a workflow execution failure.

!!! note "Investigating errors"
	To investigate failed executions, you can:

	* Review your [Executions](/workflows/executions/), for a [single workflow](/workflows/executions/single-workflow-executions/) or [all workflows you have access to](/workflows/executions/all-executions/). You can [load data from previous execution](/workflows/executions/debug/) into your current workflow.
	* Enable [Log streaming](/log-streaming/).

## Create and set an error workflow

For each workflow, you can set an error workflow in **Workflow Settings**. It runs if an execution fails. This means you can, for example, send email or Slack alerts when a workflow execution errors. The error workflow must start with the [Error Trigger](/integrations/builtin/core-nodes/n8n-nodes-base.errortrigger/).

You can use the same error workflow for multiple workflows.

--8<-- "_snippets/flow-logic/create-set-error-workflow.md"

## Error data

The default error data received by the Error Trigger is:

```json
[
	{
		"execution": {
			"id": "231",
			"url": "https://n8n.example.com/execution/231",
			"retryOf": "34",
			"error": {
				"message": "Example Error Message",
				"stack": "Stacktrace"
			},
			"lastNodeExecuted": "Node With Error",
			"mode": "manual"
		},
		"workflow": {
			"id": "1",
			"name": "Example Workflow"
		}
	}
]

```

All information is always present, except:

- `execution.id`: requires the execution to be saved in the database.
- `execution.url`: requires the execution to be saved in the database.
- `execution.retryOf`: only present when the execution is a retry of a failed execution.

## Cause a workflow execution failure using Stop And Error

When you create and set an error workflow, n8n runs it when an execution fails. Usually, this is due to things like errors in node settings, or the workflow running out of memory.

You can add the [Stop And Error](/integrations/builtin/core-nodes/n8n-nodes-base.stopanderror/) node to your workflow to force executions to fail under your chosen circumstances, and trigger the error workflow.
