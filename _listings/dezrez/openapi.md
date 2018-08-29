swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/coreplatformstate/platformissue:
    post:
      summary: Allows business workflows to post system issues to the platform state
        service.
      description: Allows business workflows to post system issues to the platform
        state service..
      operationId: CorePlatformState_PostPlatformIssueByalertDataContract
      x-api-path-slug: apicoreplatformstateplatformissue-post
      parameters:
      - in: body
        name: alertDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - Business
      - Workflows
      - To
      - Post
      - System
      - Issues
      - To
      - Platform
      - State
      - Service
  /api/workflow/triggers:
    get:
      summary: Lists the available triggers that are able to start workflows.
      description: Lists the available triggers that are able to start workflows..
      operationId: Workflow_GetTriggerTypes
      x-api-path-slug: apiworkflowtriggers-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Available
      - Triggers
      - That
      - Are
      - Able
      - To
      - Start
      - Workflows
  /api/workflow/listWorkflows:
    get:
      summary: Lists available workflows
      description: Lists available workflows.
      operationId: Workflow_ListWorkflowsByskipBytake
      x-api-path-slug: apiworkflowlistworkflows-get
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
      - Lists
      - Available
      - Workflows
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