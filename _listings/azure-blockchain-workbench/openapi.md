swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 1
info:
  title: Azure Blockchain Workbench REST API
  description: the-azure-blockchain-workbench-rest-api-is-a-workbench-extensibility-point-which-allows-developers-to-create-and-manage-blockchain-applications-manage-users-and-organizations-within-a-consortium-integrate-blockchain-applications-into-services-and-platforms-perform-transactions-on-a-blockchain-and-retrieve-transactional-and-contract-data-from-a-blockchain-
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
  /api/v1/applications/workflows/{workflowId}:
    get:
      summary: Get Applications Workflows
      description: |-
        Get a workflow matching a specific workflow ID.
                     Users who are Workbench administrators get the workflow. Non-Workbench administrators get the workflow if they
                     have at least one associated application role or is associated with a smart contract instance role.
      operationId: WorkflowGet
      x-api-path-slug: apiv1applicationsworkflowsworkflowid-get
      parameters:
      - in: path
        name: workflowId
        description: The id of the workflow
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Workflows