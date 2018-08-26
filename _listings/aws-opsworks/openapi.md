---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeDeployments:
    get:
      summary: Describe Deployments
      description: Requests a description of a specified set of deployments.
      operationId: describeDeployments
      x-api-path-slug: actiondescribedeployments-get
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      - in: query
        name: DeploymentIds
        description: An array of deployment IDs to be described
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Deployments
  /?Action=CreateDeployment:
    get:
      summary: Create Deployment
      description: Runs deployment or stack commands.
      operationId: createDeployment
      x-api-path-slug: actioncreatedeployment-get
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      - in: query
        name: Command
        description: A DeploymentCommand object that specifies the deployment command
          and any      associated arguments
        type: string
      - in: query
        name: Comment
        description: A user-defined comment
        type: string
      - in: query
        name: CustomJson
        description: A string that contains user-defined, custom JSON
        type: string
      - in: query
        name: InstanceIds
        description: The instance IDs for the deployment targets
        type: string
      - in: query
        name: LayerIds
        description: The layer IDs for the deployment targets
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment
---