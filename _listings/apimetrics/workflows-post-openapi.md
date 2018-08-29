---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 0
info:
  title: APIMetrics Create new Authentication Settings
  version: 1.0.0
  description: Create new Authentication Settings
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deployments/workflow/{workflow_id}:
    get:
      summary: Get all Deployments for a Workflow
      description: Get all Deployments for a Workflow
      operationId: getAllDeploymentForAWorkflow
      x-api-path-slug: deploymentsworkflowworkflow-id-get
      parameters:
      - in: path
        name: workflow_id
        description: ID of the Workflow
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
      - Workflow
      - Workflow
  /workflows/:
    get:
      summary: List all Workflows
      description: List all Workflows
      operationId: listAllWorkflows
      x-api-path-slug: workflows-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
    post:
      summary: Create new Authentication Settings
      description: Create new Authentication Settings
      operationId: createNewAuthenticationSettings
      x-api-path-slug: workflows-post
      parameters:
      - in: body
        name: body
        description: '{     meta: {         name: Minimal Auth Settings name,         domain:
          httpbin'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
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