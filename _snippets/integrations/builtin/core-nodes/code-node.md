The Code node allows you to write custom JavaScript or Python and run it as a step in your workflow.

!!! note "Function and Function Item nodes"
	The Code node replaces the Function and Function Item nodes from version 0.198.0 onwards. If you're using an older version of n8n, you can still view the [Function node documentation](https://github.com/n8n-io/n8n-docs/blob/67935ad2528e2e30d7984ea917e4af2910a096ec/docs/integrations/builtin/core-nodes/n8n-nodes-base.function.md){:target=_blank .external-link} and [Function Item node documentation](https://github.com/n8n-io/n8n-docs/blob/67935ad2528e2e30d7984ea917e4af2910a096ec/docs/integrations/builtin/core-nodes/n8n-nodes-base.functionItem.md){:target=_blank .external-link}.

## Usage

How to use the Code node.

### Choose a mode

There are two modes:

* **Run Once for All Items**: this is the default. When your workflow runs, the code in the code node executes once, regardless of how many input items there are.
* **Run Once for Each Item**: choose this if you want your code to run for every input item.

## JavaScript

The Code node supports Node.js.

### Supported JavaScript features

The Code node supports:

* Promises. Instead of returning the items directly, you can return a promise which resolves accordingly.
* Writing to your browser console using `console.log`. This is useful for debugging and troubleshooting your workflows.

### External libraries

If you self-host n8n, you can import and use built-in and external npm modules in the Code node. To learn how to enable external modules, refer the [Configuration](/hosting/configuration/#use-built-in-and-external-modules-in-the-code-node) guide.

### Use AI in the Code node to generate JavaScript

!!! info "Experimental feature with limited availability"
	Available on n8n Cloud from version [TODO].  
	Python isn't supported.

--8<-- "_snippets/code-examples/ai-how-to.md"

Refer to [Generate code with ChatGPT](/code-examples/ai-code/) for more information on using ChatGPT to generate code in n8n.

## Python

n8n added Python support in version 1.0. It doesn't include a Python executable. Instead, n8n provides Python support using [Pyodide](https://pyodide.org/en/stable/){:target=_blank .external-link}, which is a port of CPython to WebAssembly. This limits the available Python packages to the [Packages included with Pyodide](https://pyodide.org/en/stable/usage/packages-in-pyodide.html#packages-in-pyodide){:target=_blank .external-link}. n8n downloads the package automatically the first time you use it.

!!! note "Slower than JavaScript"
	The Code node takes longer to process Python than JavaScript. This is due to the additional compilation steps.

### File system and HTTP requests

You can't access the file system or make HTTP requests using Python. Use the following nodes instead:

* [Read Binary Files](/integrations/builtin/core-nodes/n8n-nodes-base.readbinaryfiles/) 
* [Write Binary File](/integrations/builtin/core-nodes/n8n-nodes-base.writebinaryfile/)
* [HTTP Request](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/)

## Coding in n8n

There are two places where you can use code in n8n: the Code node and the expressions editor. When using either area, there are some key concepts you need to know, as well as some built-in methods and variables to help with common tasks.

### Key concepts

When working with the Code node, you need to understand the following concepts:

* [Data structure](/data/data-structure/): understand the data you receive in the Code node, and requirements for outputting data from the node.
* [Item linking](/data/data-mapping/data-item-linking/): learn how data items work, and how to link to items from previous nodes. You need to handle item linking in your code when the number of input and output items doesn't match.

### Built-in methods and variables

n8n includes built-in methods and variables. These provide support for:

* Accessing specific item data
* Accessing data about workflows, executions, and your n8n environment
* Convenience variables to help with data and time

Refer to [methods and variables](/code-examples/methods-variables-reference/) for more information.


