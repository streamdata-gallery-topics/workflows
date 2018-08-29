{
  "info": {
    "name": "Azure Logic Apps API Workflows List By Subscription",
    "_postman_id": "4deb7ad6-3900-4df1-8f60-e51c981d58e4",
    "description": "Gets a list of workflows by subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflows subscription",
      "item": [
        {
          "id": "7494d777-25e7-4f38-a70e-1f49ce5336fd",
          "name": "Workflows_ListBySubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Logic/workflows"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Gets a list of workflows by subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dca9138-6965-4836-aa35-336906de13f8"
            }
          ]
        }
      ]
    }
  ]
}