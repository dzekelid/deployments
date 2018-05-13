---
name: Azure Resource Manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: ""
tags:
- Resources
- Microsoft
- Links
- Deployment
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/apis.yaml
specificationVersion: "0.14"
apis:
- name: Azure Resource Manager API
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: ""
  baseURL: ://management.azure.com//
  tags: Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-resources-deployments-get.md
- name: Azure Resource Manager API Deletes a deployment from the deployment history.
  description: A template deployment that is currently running cannot be deleted.
    Deleting a template deployment removes the associated deployment operations. Deleting
    a template deployment does not affect the state of the resource group. This is
    an asynchronous operation that returns a status of 202 until the template deployment
    is successfully deleted. The Location response header contains the URI that is
    used to obtain the status of the process. While the process is running, a call
    to the URI in the Location header returns a status of 202. When the process finishes,
    the URI in the Location header returns a status of 204 on success. If the asynchronous
    request failed, the URI in the Location header returns an error-level status code.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: http:://management.azure.com//
  tags: Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-resources-deployments-deploymentname-delete.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-resources-deployments-deploymentname-delete-postman.md
x-common:
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---