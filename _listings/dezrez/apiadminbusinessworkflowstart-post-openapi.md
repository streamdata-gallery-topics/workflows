---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Starts a workflow with the given parameters.
  version: 1.0.0
  description: Starts a workflow with the given parameters..
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