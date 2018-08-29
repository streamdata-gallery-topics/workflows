---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get all workflows
  description: |-
    Returns all workflows in Jira or a single workflow.

    If the `workflowName` parameter is specified, a workflow will be returned as an object (not in an array). Otherwise, an array of workflow objects will be returned.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/workflow:
    get:
      summary: Get all workflows
      description: |-
        Returns all workflows in Jira or a single workflow.

        If the `workflowName` parameter is specified, a workflow will be returned as an object (not in an array). Otherwise, an array of workflow objects will be returned.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowsResource.getAllWorkflows_get
      x-api-path-slug: api2workflow-get
      parameters:
      - in: query
        name: workflowName
        description: The name of the workflow to be returned
      responses:
        200:
          description: OK
      tags:
      - Workflows
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---