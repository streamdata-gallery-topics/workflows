swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 1
info:
  title: LogicManagementClient
  description: rest-api-for-azure-logic-apps-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}:
    get:
      summary: Workflows Get
      description: Gets a workflow.
      operationId: Workflows_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows
    put:
      summary: Workflows Create Or Update
      description: Creates or updates a workflow.
      operationId: Workflows_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: body
        name: workflow
        description: The workflow
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows
    patch:
      summary: Workflows Update
      description: Updates a workflow.
      operationId: Workflows_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-patch
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: body
        name: workflow
        description: The workflow
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows
    delete:
      summary: Workflows Delete
      description: Deletes a workflow.
      operationId: Workflows_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows