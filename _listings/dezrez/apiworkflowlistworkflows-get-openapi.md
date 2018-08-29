---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Lists available workflows
  version: 1.0.0
  description: Lists available workflows.
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
    delete:
      summary: Terminates a running workflow instance.
      description: Terminates a running workflow instance..
      operationId: BusinessWorkflow_TerminateWorkflowInstanceByworkflowNameByworkflowInstanceHandleByreason
      x-api-path-slug: apiadminbusinessworkflowworkflowname-delete
      parameters:
      - in: query
        name: reason
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: workflowInstanceHandle
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Terminates
      - Running
      - Workflow
      - Instance
  /api/coreplatformstate/reportMigration/{migrationId}:
    post:
      summary: Reports that a data migration has been shedueled - used by workflow
      description: Reports that a data migration has been shedueled - used by workflow.
      operationId: CorePlatformState_ReportMigrationStateBymigrationId
      x-api-path-slug: apicoreplatformstatereportmigrationmigrationid-post
      parameters:
      - in: path
        name: migrationId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reports
      - That
      - Data
      - Migration
      - Has
      - Been
      - Shedueled
      - '-'
      - Used
      - By
      - Workflow
  /api/workflow/start:
    post:
      summary: Starts a workflow with the given parameters.
      description: Starts a workflow with the given parameters..
      operationId: Workflow_StartWorkflowByinvokeCommand
      x-api-path-slug: apiworkflowstart-post
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
  /api/workflow/{workflowName}:
    get:
      summary: Lists instances of a given workflow
      description: Lists instances of a given workflow.
      operationId: Workflow_ListWorkflowInstancesByworkflowNameByskipBytake
      x-api-path-slug: apiworkflowworkflowname-get
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
    delete:
      summary: Terminates a running workflow instance.
      description: Terminates a running workflow instance..
      operationId: Workflow_TerminateWorkflowInstanceByworkflowNameByworkflowInstanceHandleByreason
      x-api-path-slug: apiworkflowworkflowname-delete
      parameters:
      - in: query
        name: reason
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: workflowInstanceHandle
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Terminates
      - Running
      - Workflow
      - Instance
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