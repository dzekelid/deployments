---
swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 0
info:
  title: Azure Resource Manager API Deploys resources to a resource group.
  description: You can provide the template and parameters directly in the request
    or link to JSON files.
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
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Resources/deployments/{deploymentName}:
    delete:
      summary: Deletes a deployment from the deployment history.
      description: A template deployment that is currently running cannot be deleted.
        Deleting a template deployment removes the associated deployment operations.
        Deleting a template deployment does not affect the state of the resource group.
        This is an asynchronous operation that returns a status of 202 until the template
        deployment is successfully deleted. The Location response header contains
        the URI that is used to obtain the status of the process. While the process
        is running, a call to the URI in the Location header returns a status of 202.
        When the process finishes, the URI in the Location header returns a status
        of 204 on success. If the asynchronous request failed, the URI in the Location
        header returns an error-level status code.
      operationId: Deployments_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-delete
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment to delete
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group with the deployment to delete
      responses:
        200:
          description: OK
      tags:
      - Deployments
    head:
      summary: Deployments Check Existence
      description: Checks whether the deployment exists.
      operationId: Deployments_CheckExistence
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-head
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment to check
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group with the deployment to check
      responses:
        200:
          description: OK
      tags:
      - Deployments
    put:
      summary: Deploys resources to a resource group.
      description: You can provide the template and parameters directly in the request
        or link to JSON files.
      operationId: Deployments_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcesdeploymentsdeploymentname-put
      parameters:
      - in: path
        name: deploymentName
        description: The name of the deployment
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Additional parameters supplied to the operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to deploy the resources to
      responses:
        200:
          description: OK
      tags:
      - Deployments
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