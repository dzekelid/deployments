---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 1
info:
  title: APImetrics Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deployments/:
    get:
      summary: List all Deployment
      description: List all Deployment
      operationId: listAllDeployments
      x-api-path-slug: deployments-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
    post:
      summary: Create a new Deployment
      description: Create a new Deployment
      operationId: createANewDeployment
      x-api-path-slug: deployments-post
      parameters:
      - in: body
        name: body
        description: '{     deployment: {         target_id: agxkZXZ-dmlhdGVzdHNyFwsSClRlc3RTZXR1cDIYgICAgKDL6gsM,          frequency:
          12,         location_id:      } }'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
  /deployments/call/{call_id}/:
    get:
      summary: Get all Deployments for an API Call
      description: Get all Deployments for an API Call
      operationId: getAllDeploymentForAPICall
      x-api-path-slug: deploymentscallcall-id-get
      parameters:
      - in: path
        name: call_id
        description: ID of the API Call
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
      - Call
      - Call
  /deployments/workflow/{workflow_id}:
    get:
      summary: Get all Deployments for a Workflow
      description: Get all Deployments for a Workflow
      operationId: getAllDeploymentForAWorkflow
      x-api-path-slug: deploymentsworkflowworkflow-id-get
      parameters:
      - in: path
        name: workflow_id
        description: ID of the Workflow
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
      - Workflow
      - Workflow
  /deployments/{id}/:
    delete:
      summary: Delete a Deployment
      description: Delete a Deployment
      operationId: deleteADeployment
      x-api-path-slug: deploymentsid-delete
      parameters:
      - in: path
        name: id
        description: ID string of deployment you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
    get:
      summary: Get an existing Deployment
      description: Get an existing Deployment
      operationId: getAnExistingDeployment
      x-api-path-slug: deploymentsid-get
      parameters:
      - in: path
        name: id
        description: ID string of deployment you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
    put:
      summary: Update an existing Deployment
      description: Update an existing Deployment
      operationId: updateAnExistingDeployment
      x-api-path-slug: deploymentsid-put
      parameters:
      - in: body
        name: body
        description: '{     deployment: {         target_id: __PARENT_ID__,          frequency:
          15,         location_id:      } }'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of deployment you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
---