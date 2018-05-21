---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API Get Deployment
  version: 1.0.0
  description: Gets information about a deployment.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BatchGetDeployments:
    get:
      summary: Batch Get Deployments
      description: Gets information about one or more deployments.
      operationId: batchGetDeployments
      x-api-path-slug: actionbatchgetdeployments-get
      parameters:
      - in: query
        name: deploymentIds
        description: A list of deployment IDs, separated by spaces
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=CreateDeployment:
    get:
      summary: Create Deployment
      description: Deploys an application revision through the specified deployment
        group.
      operationId: createDeployment
      x-api-path-slug: actioncreatedeployment-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: autoRollbackConfiguration
        description: Configuration information for an automatic rollback that is added
          when a deployment            is created
        type: string
      - in: query
        name: deploymentConfigName
        description: The name of a deployment configuration associated with the applicable
          IAM user or            AWS account
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of the deployment group
        type: string
      - in: query
        name: description
        description: A comment about the deployment
        type: string
      - in: query
        name: ignoreApplicationStopFailures
        description: If set to true, then if the deployment causes the ApplicationStop
          deployment            lifecycle event to an instance to fail, the deployment
          to that instance will not be            considered to have failed at that
          point and will continue on to the BeforeInstall            deployment lifecycle
          event
        type: string
      - in: query
        name: revision
        description: The type and location of the revision to deploy
        type: string
      - in: query
        name: updateOutdatedInstancesOnly
        description: Indicates whether to deploy to all instances or only to instances
          that are not            running the latest application revision
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=CreateDeploymentConfig:
    get:
      summary: Create Deployment Config
      description: Creates a deployment configuration.
      operationId: createDeploymentConfig
      x-api-path-slug: actioncreatedeploymentconfig-get
      parameters:
      - in: query
        name: deploymentConfigName
        description: The name of the deployment configuration to create
        type: string
      - in: query
        name: minimumHealthyHosts
        description: The minimum number of healthy instances that should be available
          at any time during            the deployment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=DeleteDeploymentConfig:
    get:
      summary: Delete Deployment Config
      description: Deletes a deployment configuration.
      operationId: deleteDeploymentConfig
      x-api-path-slug: actiondeletedeploymentconfig-get
      parameters:
      - in: query
        name: deploymentConfigName
        description: The name of a deployment configuration associated with the applicable
          IAM user or            AWS account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=GetDeployment:
    get:
      summary: Get Deployment
      description: Gets information about a deployment.
      operationId: getDeployment
      x-api-path-slug: actiongetdeployment-get
      parameters:
      - in: query
        name: deploymentId
        description: A deployment ID associated with the applicable IAM user or AWS
          account
        type: string
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