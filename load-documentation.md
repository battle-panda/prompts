name: load-documentation
description: Use hyaline to load relevant documentation into context
arguments:
  - name: task
    description: A description of the task being performed
    required: true
resources:
  - path: ./resources/documentation-summary.template.md
    name: documentation-summary-template
---

Based on the following task, use the hyaline MCP server to get relevant documentation.

Task: ${task}

Use the provided documentation-summary-template to summarize the documentation that was retrieved.
