---
swagger: "2.0"
x-collection-name: AppVeyor CI
x-complete: 0
info:
  title: App Veyor Get Environments Deploymentenvironmentid Deployments
  description: Get environments deploymentenvironmentid deployments.
  termsOfService: https://www.appveyor.com/terms-of-service/
  contact:
    name: AppVeyor Team
    url: https://www.appveyor.com/about/
    email: team@appveyor.com
  version: 0.20170106.0
host: ci.appveyor.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deployments:
    post:
      summary: Post Deployments
      description: Post deployments.
      operationId: postDeployments
      x-api-path-slug: deployments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /deployments/stop:
    delete:
      summary: Delete Deployments Stop
      description: Delete deployments stop.
      operationId: deleteDeploymentsStop
      x-api-path-slug: deploymentsstop-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Deployments
      - Stop
  /deployments/{deploymentId}:
    get:
      summary: Get Deployments Deploymentid
      description: Get deployments deploymentid.
      operationId: getDeploymentsDeployment
      x-api-path-slug: deploymentsdeploymentid-get
      responses:
        200:
          description: OK
      tags:
      - Deployments
      - DeploymentId
    parameters:
      summary: Parameters Deployments Deploymentid
      description: Parameters deployments deploymentid.
      operationId: parametersDeploymentsDeployment
      x-api-path-slug: deploymentsdeploymentid-parameters
      responses:
        200:
          description: OK
      tags:
      - Deployments
      - DeploymentId
  /environments/{deploymentEnvironmentId}/deployments:
    get:
      summary: Get Environments Deploymentenvironmentid Deployments
      description: Get environments deploymentenvironmentid deployments.
      operationId: getEnvironmentsDeploymentenvironmentDeployments
      x-api-path-slug: environmentsdeploymentenvironmentiddeployments-get
      responses:
        200:
          description: OK
      tags:
      - Environments
      - DeploymentEnvironmentId
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