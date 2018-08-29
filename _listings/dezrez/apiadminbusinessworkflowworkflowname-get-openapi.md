---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Lists instances of a given workflow
  version: 1.0.0
  description: Lists instances of a given workflow.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/admin/businessworkflow/start:
    post:
      summary: Starts a workflow with the given parameters.
      description: Starts a workflow with the given parameters..
      operationId: BusinessWorkflow_StartWorkflowByinvokeCommand
      x-api-path-slug: apiadminbusinessworkflowstart-post
      parameters:
      - in: body
        name: invokeCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Workflow
      - Given
      - Parameters
  /api/admin/businessworkflow/listWorkflows:
    get:
      summary: Starts a workflow with the given parameters.
      description: Starts a workflow with the given parameters..
      operationId: BusinessWorkflow_ListWorkflowsByskipBytake
      x-api-path-slug: apiadminbusinessworkflowlistworkflows-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
        description: Used for paging results
      - in: query
        name: take
        description: Used for paging results
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Workflow
      - Given
      - Parameters
  /api/admin/businessworkflow/{workflowName}:
    get:
      summary: Lists instances of a given workflow
      description: Lists instances of a given workflow.
      operationId: BusinessWorkflow_ListWorkflowInstancesByworkflowNameByskipBytake
      x-api-path-slug: apiadminbusinessworkflowworkflowname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
      - in: query
        name: take
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Instances
      - Of
      - Given
      - Workflow
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