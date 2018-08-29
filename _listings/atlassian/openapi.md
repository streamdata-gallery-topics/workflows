swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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