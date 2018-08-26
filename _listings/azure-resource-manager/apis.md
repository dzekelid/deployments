---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Deployments
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: SubscriptionClient - Deletes a deployment from the deployment history.
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-delete
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
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-delete-openapi.md
- name: SubscriptionClient - Deployments Check Existence
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-head
  description: Checks whether the deployment exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-head-openapi.md
- name: SubscriptionClient - Deployments Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-get
  description: Gets a deployment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-get-openapi.md
- name: SubscriptionClient - Cancels a currently running template deployment.
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnamecancel-post
  description: You can cancel a deployment only if the provisioningState is Accepted
    or Running. After the deployment is canceled, the provisioningState is set to
    Canceled. Canceling a template deployment stops the currently running template
    deployment and leaves the resource group partially deployed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnamecancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnamecancel-post-openapi.md
- name: SubscriptionClient - Deployments Export Template
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnameexporttemplate-post
  description: Exports the template used for specified deployment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnameexporttemplate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentnameexporttemplate-post-openapi.md
- name: SubscriptionClient - Deployments List
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeployments-get
  description: Get all the deployments for a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeployments-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.resource.health.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.resource.manager.stack.network
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---