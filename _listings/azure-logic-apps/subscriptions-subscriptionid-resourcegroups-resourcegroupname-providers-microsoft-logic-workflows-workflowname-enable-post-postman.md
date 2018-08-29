{
  "info": {
    "name": "Azure Logic Apps API Workflows Enable",
    "_postman_id": "0800d318-4197-4d51-90ae-dad77338bc80",
    "description": "Enables a workflow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflows enable",
      "item": [
        {
          "id": "f86927e9-1497-4705-91b3-c8833f845428",
          "name": "Workflows_Enable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/workflows/:workflowName/enable"
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
            "description": "Enables a workflow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdf53723-6b8b-4453-877a-df6cde988076"
            }
          ]
        }
      ]
    }
  ]
}