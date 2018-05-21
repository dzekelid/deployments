---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 0
info:
  title: APIMetrics Delete a Deployment
  version: 1.0.0
  description: Delete a Deployment
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