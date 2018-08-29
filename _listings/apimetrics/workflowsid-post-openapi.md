---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 0
info:
  title: APIMetrics Trigger a Workflow to run now
  version: 1.0.0
  description: Trigger a Workflow to run now
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
  /workflows/{id}/:
    delete:
      summary: Delete a Workflow
      description: Delete a Workflow
      operationId: deleteAWorkflow
      x-api-path-slug: workflowsid-delete
      parameters:
      - in: path
        name: id
        description: ID string of Workflow you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
    get:
      summary: Get an existing Workflow
      description: Get an existing Workflow
      operationId: getAnExistingWorkflow
      x-api-path-slug: workflowsid-get
      parameters:
      - in: path
        name: id
        description: ID string of Workflow you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
    post:
      summary: Trigger a Workflow to run now
      description: Trigger a Workflow to run now
      operationId: triggerAWorkflowToRunNow
      x-api-path-slug: workflowsid-post
      parameters:
      - in: body
        name: body
        description: '{     location_id: ,     context: {         foo: 1234,         bar:
          %%RESULT_ID%%,         datum: %%DATETIME%%     } }'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of Workflow you are updating
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