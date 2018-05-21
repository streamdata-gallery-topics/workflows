---
name: Azure Logic Apps
x-slug: azure-logic-apps
description: You can connect apps, data, and devices anywhere&mdash;on-premises or
  in the cloud&mdash;with our large ecosystem of software as a service (SaaS) and
  cloud-based connectors that includes Salesforce, Office 365, Twitter, Dropbox, Google
  services, and more. Its never been easier to access data and keep your disparate
  systems up-to-date, in real-time. New connectors are being added to the Azure Marketplace
  all of the time.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
x-kinRank: "10"
x-alexaRank: ""
tags: Workflows
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Logic Apps API Workflows List By Subscription
  x-api-slug: azure-logic-apps-api
  description: Gets a list of workflows by subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Logic/workflows
  tags: Workflows Subscription
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidprovidersmicrosoftlogicworkflows-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidprovidersmicrosoftlogicworkflows-get-openapi.md
- name: Azure Logic Apps API Workflows List By Resource Group
  x-api-slug: azure-logic-apps-api
  description: Gets a list of workflows by resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows
  tags: Workflows Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflows-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflows-get-openapi.md
- name: Azure Logic Apps API Workflows Get
  x-api-slug: azure-logic-apps-api
  description: Gets a workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}
  tags: Workflows
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-get-openapi.md
- name: Azure Logic Apps API Workflows Create Or Update
  x-api-slug: azure-logic-apps-api
  description: Creates or updates a workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}
  tags: Workflows
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-put-openapi.md
- name: Azure Logic Apps API Workflows Update
  x-api-slug: azure-logic-apps-api
  description: Updates a workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}
  tags: Workflows
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-patch-openapi.md
- name: Azure Logic Apps API Workflows Delete
  x-api-slug: azure-logic-apps-api
  description: Deletes a workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}
  tags: Workflows
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-delete-openapi.md
- name: Azure Logic Apps API Workflows Disable
  x-api-slug: azure-logic-apps-api
  description: Disables a workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/disable
  tags: Workflows Disable
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamedisable-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamedisable-post-openapi.md
- name: Azure Logic Apps API Workflows Enable
  x-api-slug: azure-logic-apps-api
  description: Enables a workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/enable
  tags: Workflows Enable
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameenable-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameenable-post-openapi.md
- name: Azure Logic Apps API Workflows Generate Upgraded Definition
  x-api-slug: azure-logic-apps-api
  description: Generates the upgraded definition for a workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/generateUpgradedDefinition
  tags: Workflows Generate Upgraded Definition
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamegenerateupgradeddefinition-post-openapi.md
- name: Azure Logic Apps API Workflows List Swagger
  x-api-slug: azure-logic-apps-api
  description: Gets an OpenAPI definition for the workflow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/listSwagger
  tags: Workflows Swagger
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamelistswagger-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamelistswagger-post-openapi.md
- name: Azure Logic Apps API Workflows Regenerate Access Key
  x-api-slug: azure-logic-apps-api
  description: Regenerates the callback URL access key for request triggers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/regenerateAccessKey
  tags: Workflows Regenerate Access Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameregenerateaccesskey-post-openapi.md
- name: Azure Logic Apps API Workflows Validate
  x-api-slug: azure-logic-apps-api
  description: Validates the workflow definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/locations/{location}/workflows/{workflowName}/validate
  tags: Workflows Validate
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogiclocationslocationworkflowsworkflownamevalidate-post-openapi.md
- name: Azure Logic Apps API
  x-api-slug: azure-logic-apps-api
  description: You can connect apps, data, and devices anywhere&mdash;on-premises
    or in the cloud&mdash;with our large ecosystem of software as a service (SaaS)
    and cloud-based connectors that includes Salesforce, Office 365, Twitter, Dropbox,
    Google services, and more. Its never been easier to access data and keep your
    disparate systems up-to-date, in real-time. New connectors are being added to
    the Azure Marketplace all of the time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-logic-apps-01-connectors.png
  humanURL: https://azure.microsoft.com/en-us/services/logic-apps/
  baseURL: ://management.azure.com//
  tags: Workflows
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/workflows/master/_listings/azure-logic-apps/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/logic-apps/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/logic-apps/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/logic-apps/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/logic-apps/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---