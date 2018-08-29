---
swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 0
info:
  title: Azure Blockchain Workbench Get Applications Workflows
  description: |-
    List all workflows of the specified blockchain application. Users who are Workbench administrators get all
                 workflows. Non-Workbench administrators get all workflows for which they have at least one associated application role
                 or are associated with a smart contract instance role.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/applications/{applicationId}/workflows:
    get:
      summary: Get Applications Workflows
      description: |-
        List all workflows of the specified blockchain application. Users who are Workbench administrators get all
                     workflows. Non-Workbench administrators get all workflows for which they have at least one associated application role
                     or are associated with a smart contract instance role.
      operationId: WorkflowsGet
      x-api-path-slug: apiv1applicationsapplicationidworkflows-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Applications
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