{
  "info": {
    "name": "Azure Logic Apps API Workflows List Swagger",
    "_postman_id": "c13a278a-0e52-46a8-86e6-943b9b3c2897",
    "description": "Gets an OpenAPI definition for the workflow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflows swagger",
      "item": [
        {
          "id": "15237605-473f-4dd3-8f0e-35ab5ac55861",
          "name": "Workflows_ListSwagger",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/workflows/:workflowName/listSwagger"
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
            "description": "Gets an OpenAPI definition for the workflow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddca08f2-af8f-4881-a01f-74813316ef6b"
            }
          ]
        }
      ]
    }
  ]
}