---
name: Azure Blockchain Workbench
x-slug: azure-blockchain-workbench
description: Azure Blockchain Workbench helps organizations build rich, integrated
  multi-party blockchain applications quickly and easily. Azure Blockchain Workbench
  REST API provides developers and information workers a way to integrate to blockchain
  applications. For example, a developer can use the REST API to enable IoT devices
  to send data to a blockchain application. Or, an information worker can use the
  REST API and Power BI to create visualization of blockchain data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
x-kinRank: "7"
x-alexaRank: ""
tags: Workflows
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-blockchain-workbench/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Blockchain Workbench REST API - Get Applications Workflows
  x-api-slug: apiv1applicationsapplicationidworkflows-get
  description: |-
    List all workflows of the specified blockchain application. Users who are Workbench administrators get all
                 workflows. Non-Workbench administrators get all workflows for which they have at least one associated application role
                 or are associated with a smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-blockchain-workbench/apiv1applicationsapplicationidworkflows-get-openapi.md
- name: Azure Blockchain Workbench REST API - Get Applications Workflows
  x-api-slug: apiv1applicationsworkflowsworkflowid-get
  description: |-
    Get a workflow matching a specific workflow ID.
                 Users who are Workbench administrators get the workflow. Non-Workbench administrators get the workflow if they
                 have at least one associated application role or is associated with a smart contract instance role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-blockchain.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
  baseURL: https:////
  tags: Blockchain, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-blockchain-workbench/apiv1applicationsworkflowsworkflowid-get-openapi.md
x-common:
- type: x-blog
  url: https://azure.microsoft.com/en-us/blog/topics/blockchain/
- type: x-blog-rss
  url: https://azurecomcdn.azureedge.net/en-us/blog/topics/blockchain/feed/
- type: x-openapi
  url: https://raw.githubusercontent.com/Azure-Samples/blockchain/master/blockchain-workbench/rest-api-samples/swagger/swagger.json
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/azure-blockchain-workbench/
- type: x-api-gallery
  url: http://azure.billing.api.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.blockchain.workbench.stack.network
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---