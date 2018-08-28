---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API List Deployment Configs
  version: 1.0.0
  description: |-
    Lists the deployment configurations with the applicable IAM user or AWS
                account.
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
  /?Action=GetDeploymentConfig:
    get:
      summary: Get Deployment Config
      description: Gets information about a deployment configuration.
      operationId: getDeploymentConfig
      x-api-path-slug: actiongetdeploymentconfig-get
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
  /?Action=ListDeploymentConfigs:
    get:
      summary: List Deployment Configs
      description: |-
        Lists the deployment configurations with the applicable IAM user or AWS
                    account.
      operationId: listDeploymentConfigs
      x-api-path-slug: actionlistdeploymentconfigs-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployment configurations
          call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=ListDeployments:
    get:
      summary: List Deployments
      description: |-
        Lists the deployments in a deployment group for an application registered with the
                    applicable IAM user or AWS account.
      operationId: listDeployments
      x-api-path-slug: actionlistdeployments-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: createTimeRange
        description: A time range (start and end) for returning a subset of the list
          of            deployments
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of an existing deployment group for the specified application
        type: string
      - in: query
        name: includeOnlyStatuses
        description: 'A subset of deployments to list by status:'
        type: string
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployments call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=StopDeployment:
    get:
      summary: Stop Deployment
      description: Attempts to stop an ongoing deployment.
      operationId: stopDeployment
      x-api-path-slug: actionstopdeployment-get
      parameters:
      - in: query
        name: autoRollbackEnabled
        description: Indicates, when a deployment is stopped, whether instances that
          have been updated            should be rolled back to the previous version
          of the application revision
        type: string
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=BatchGetDeploymentGroups:
    get:
      summary: Batch Get Deployment Groups
      description: Gets information about one or more deployment groups.
      operationId: batchGetDeploymentGroups
      x-api-path-slug: actionbatchgetdeploymentgroups-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: deploymentGroupNames
        description: The deployment groups names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=BatchGetDeploymentInstances:
    get:
      summary: Batch Get Deployment Instances
      description: |-
        Gets information about one or more instance that are part of a deployment
                    group.
      operationId: batchGetDeploymentInstances
      x-api-path-slug: actionbatchgetdeploymentinstances-get
      parameters:
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      - in: query
        name: instanceIds
        description: The unique IDs of instances in the deployment group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Instances
  /?Action=CreateDeploymentGroup:
    get:
      summary: Create Deployment Group
      description: |-
        Creates a deployment group to which application revisions will be
                    deployed.
      operationId: createDeploymentGroup
      x-api-path-slug: actioncreatedeploymentgroup-get
      parameters:
      - in: query
        name: alarmConfiguration
        description: Information to add about Amazon CloudWatch alarms when the deployment
          group is            created
        type: string
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: autoRollbackConfiguration
        description: Configuration information for an automatic rollback that is added
          when a deployment            group is created
        type: string
      - in: query
        name: autoScalingGroups
        description: A list of associated Auto Scaling groups
        type: string
      - in: query
        name: deploymentConfigName
        description: If specified, the deployment configuration name can be either
          one of the predefined            configurations provided with AWS CodeDeploy
          or a custom deployment configuration that            you create by calling
          the create deployment configuration operation
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of a new deployment group for the specified application
        type: string
      - in: query
        name: ec2TagFilters
        description: The Amazon EC2 tags on which to filter
        type: string
      - in: query
        name: onPremisesInstanceTagFilters
        description: The on-premises instance tags on which to filter
        type: string
      - in: query
        name: serviceRoleArn
        description: A service role ARN that allows AWS CodeDeploy to act on the users
          behalf when            interacting with AWS services
        type: string
      - in: query
        name: triggerConfigurations
        description: Information about triggers to create when the deployment group
          is created
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=DeleteDeploymentGroup:
    get:
      summary: Delete Deployment Group
      description: Deletes a deployment group.
      operationId: deleteDeploymentGroup
      x-api-path-slug: actiondeletedeploymentgroup-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of an existing deployment group for the specified application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=GetDeploymentGroup:
    get:
      summary: Get Deployment Group
      description: Gets information about a deployment group.
      operationId: getDeploymentGroup
      x-api-path-slug: actiongetdeploymentgroup-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of an existing deployment group for the specified application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=GetDeploymentInstance:
    get:
      summary: Get Deployment Instance
      description: Gets information about an instance as part of a deployment.
      operationId: getDeploymentInstance
      x-api-path-slug: actiongetdeploymentinstance-get
      parameters:
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      - in: query
        name: instanceId
        description: The unique ID of an instance in the deployment group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Instances
  /?Action=ListDeploymentGroups:
    get:
      summary: List Deployment Groups
      description: |-
        Lists the deployment groups for an application registered with the applicable IAM
                    user or AWS account.
      operationId: listDeploymentGroups
      x-api-path-slug: actionlistdeploymentgroups-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployment groups
          call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=ListDeploymentInstances:
    get:
      summary: List Deployment Instances
      description: |-
        Lists the instance for a deployment associated with the applicable IAM user or AWS
                    account.
      operationId: listDeploymentInstances
      x-api-path-slug: actionlistdeploymentinstances-get
      parameters:
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      - in: query
        name: instanceStatusFilter
        description: 'A subset of instances to list by status:'
        type: string
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployment instances
          call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Instances
  /?Action=RegisterApplicationRevision:
    get:
      summary: Register Application Revision
      description: Registers with AWS CodeDeploy a revision for the specified application.
      operationId: registerApplicationRevision
      x-api-path-slug: actionregisterapplicationrevision-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: description
        description: A comment about the revision
        type: string
      - in: query
        name: revision
        description: Information about the application revision to register, including
          type and            location
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Revisions
  /?Action=UpdateDeploymentGroup:
    get:
      summary: Update Deployment Group
      description: Changes information about a deployment group.
      operationId: updateDeploymentGroup
      x-api-path-slug: actionupdatedeploymentgroup-get
      parameters:
      - in: query
        name: alarmConfiguration
        description: Information to add or change about Amazon CloudWatch alarms when
          the deployment            group is updated
        type: string
      - in: query
        name: applicationName
        description: The application name corresponding to the deployment group to
          update
        type: string
      - in: query
        name: autoRollbackConfiguration
        description: Information for an automatic rollback configuration that is added
          or changed when a            deployment group is updated
        type: string
      - in: query
        name: autoScalingGroups
        description: The replacement list of Auto Scaling groups to be included in
          the deployment group,            if you want to change them
        type: string
      - in: query
        name: currentDeploymentGroupName
        description: The current name of the deployment group
        type: string
      - in: query
        name: deploymentConfigName
        description: The replacement deployment configuration name to use, if you
          want to change            it
        type: string
      - in: query
        name: ec2TagFilters
        description: The replacement set of Amazon EC2 tags on which to filter, if
          you want to change            them
        type: string
      - in: query
        name: newDeploymentGroupName
        description: The new name of the deployment group, if you want to change it
        type: string
      - in: query
        name: onPremisesInstanceTagFilters
        description: The replacement set of on-premises instance tags on which to
          filter, if you want to            change them
        type: string
      - in: query
        name: serviceRoleArn
        description: A replacement ARN for the service role, if you want to change
          it
        type: string
      - in: query
        name: triggerConfigurations
        description: Information about triggers to change when the deployment group
          is updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
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