---
swagger: "2.0"
x-collection-name: Google Cloud Deployment Manager
x-complete: 1
info:
  title: Google Cloud Deployment Manager
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/deployments:
    get:
      summary: Get Deployments
      description: Lists all deployments for a given project.
      operationId: deploymentmanager.deployments.list
      x-api-path-slug: projectglobaldeployments-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
    post:
      summary: Create Deployment
      description: Creates a deployment and all of the resources described by the
        deployment manifest.
      operationId: deploymentmanager.deployments.insert
      x-api-path-slug: projectglobaldeployments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: preview
        description: If set to true, creates a deployment and creates shell resources
          but does not actually instantiate these resources
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
  /{project}/global/deployments/{deployment}:
    delete:
      summary: Delete Deployment
      description: Deletes a deployment and all of the resources in the deployment.
      operationId: deploymentmanager.deployments.delete
      x-api-path-slug: projectglobaldeploymentsdeployment-delete
      parameters:
      - in: query
        name: deletePolicy
        description: Sets the policy to use for deleting resources
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
    get:
      summary: Get Deployment
      description: Gets information about a specific deployment.
      operationId: deploymentmanager.deployments.get
      x-api-path-slug: projectglobaldeploymentsdeployment-get
      parameters:
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
    patch:
      summary: update Deployment
      description: Updates a deployment and all of the resources described by the
        deployment manifest. This method supports patch semantics.
      operationId: deploymentmanager.deployments.patch
      x-api-path-slug: projectglobaldeploymentsdeployment-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: createPolicy
        description: Sets the policy to use for creating new resources
      - in: query
        name: deletePolicy
        description: Sets the policy to use for deleting resources
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: query
        name: preview
        description: If set to true, updates the deployment and creates and updates
          the shell resources but does not actually alter or instantiate these resources
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
    put:
      summary: update Deployment
      description: Updates a deployment and all of the resources described by the
        deployment manifest.
      operationId: deploymentmanager.deployments.update
      x-api-path-slug: projectglobaldeploymentsdeployment-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: createPolicy
        description: Sets the policy to use for creating new resources
      - in: query
        name: deletePolicy
        description: Sets the policy to use for deleting resources
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: query
        name: preview
        description: If set to true, updates the deployment and creates and updates
          the shell resources but does not actually alter or instantiate these resources
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
  /{project}/global/deployments/{deployment}/cancelPreview:
    post:
      summary: Cancel Preview
      description: Cancels and removes the preview currently associated with the deployment.
      operationId: deploymentmanager.deployments.cancelPreview
      x-api-path-slug: projectglobaldeploymentsdeploymentcancelpreview-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
  /{project}/global/deployments/{deployment}/stop:
    post:
      summary: Stop Deployment
      description: Stops an ongoing operation. This does not roll back any work that
        has already been completed, but prevents any new work from being started.
      operationId: deploymentmanager.deployments.stop
      x-api-path-slug: projectglobaldeploymentsdeploymentstop-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Deployment
---