---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Runtime Deploy the specified orchestration workflow file
    to the Orchestration Engine.
  version: 1.0.0
  description: This API will deploy the BPMN file associated with the specified orchestration
    configuration to the Orchestration Engine in preparation for orchestration execution.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/execution/orchestrations/{orchConfigId}/deployment:
    post:
      summary: Deploy the specified orchestration workflow file to the Orchestration
        Engine.
      description: This API will deploy the BPMN file associated with the specified
        orchestration configuration to the Orchestration Engine in preparation for
        orchestration execution.
      operationId: retrieveAndDeployBpmn
      x-api-path-slug: apiv2executionorchestrationsorchconfigiddeployment-post
      parameters:
      - in: path
        name: orchConfigId
        description: orchestration configuration id
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Deploy
      - Specified
      - Orchestration
      - Workflow
      - File
      - To
      - Orchestration
      - Engine
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