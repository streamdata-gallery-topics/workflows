{
  "info": {
    "name": "Azure Logic Apps API Workflows Disable",
    "_postman_id": "d53cf0f6-d509-4858-97a8-7a96d034ea62",
    "description": "Disables a workflow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflows disable",
      "item": [
        {
          "id": "f9036099-78e7-4b30-9deb-4860df5000ca",
          "name": "Workflows_Disable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/workflows/:workflowName/disable"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Disables a workflow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fba93eb8-2003-4a2a-b2fb-9945bd3d5766"
            }
          ]
        }
      ]
    }
  ]
}