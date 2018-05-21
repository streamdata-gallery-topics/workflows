---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 1
info:
  title: APImetrics Merged API
  version: 1.0.0
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
    put:
      summary: Create a new Workflow
      description: Create a new Workflow
      operationId: createANewWorkflow
      x-api-path-slug: workflowsid-put
      parameters:
      - in: body
        name: body
        description: '{     workflow: {         call_ids: [             agxkZXZ-dmlhdGVzdHNyFwsSClRlc3RTZXR1cDIYgICAgKDL6gsM,             agxkZXZ-dmlhdGVzdHNyFwsSClRlc3RTZXR1cDIYgICAgKDL6gsM         ],         handle_cookies:
          true     } }'
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
---