---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Workflows List By Subscription
  description: Gets a list of workflows by subscription.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Logic/workflows:
    get:
      summary: Workflows List By Subscription
      description: Gets a list of workflows by subscription.
      operationId: Workflows_ListBySubscription
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftlogicworkflows-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Workflows Subscription
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