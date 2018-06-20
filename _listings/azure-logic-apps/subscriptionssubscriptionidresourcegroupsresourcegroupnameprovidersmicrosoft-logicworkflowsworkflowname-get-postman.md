{
  "info": {
    "name": "Azure Logic Apps API Workflows Get",
    "_postman_id": "39c07bbd-8d65-4f11-a8da-d0254a3883ae",
    "description": "Gets a workflow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflows",
      "item": [
        {
          "id": "95d9675a-d8d6-4357-b91a-5a844187acfb",
          "name": "Workflows_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/workflows/:workflowName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "workflowName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a workflow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73d7dfec-5209-44af-a2db-60b93454a2e8"
            }
          ]
        }
      ]
    }
  ]
}