---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Delete Projects Deploy Keys Key Disable
  version: 1.0.0
  description: Delete projects deploy keys key disable.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/deployments:
    get:
      summary: Get Projects Deployments
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdDeployments
      x-api-path-slug: v3projectsiddeployments-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        2:
          description: Successful response
        200:
          description: OK
      tags:
      - Projects
      - Deployments
  /v3/projects/{id}/deployments/{deployment_id}:
    get:
      summary: Get Projects Deployments Deployment
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdDeploymentsDeploymentId
      x-api-path-slug: v3projectsiddeploymentsdeployment-id-get
      parameters:
      - in: path
        name: deployment_id
        description: The deployment ID
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deployments
      - Deployment
  /v3/projects/{id}/deploy_keys:
    get:
      summary: Get Projects Deploy Keys
      description: Get a specific project's deploy keys
      operationId: getV3ProjectsIdDeployKeys
      x-api-path-slug: v3projectsiddeploy-keys-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
    post:
      summary: Post Projects Deploy Keys
      description: Add new deploy key to currently authenticated user
      operationId: postV3ProjectsIdDeployKeys
      x-api-path-slug: v3projectsiddeploy-keys-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: formData
        name: key
        description: The new deploy key
      - in: formData
        name: title
        description: The name of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
  /v3/projects/{id}/deploy_keys/{key_id}:
    get:
      summary: Get Projects Deploy Keys Key
      description: Get projects deploy keys key.
      operationId: getV3ProjectsIdDeployKeysKeyId
      x-api-path-slug: v3projectsiddeploy-keyskey-id-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
    delete:
      summary: Delete Projects Deploy Keys Key
      description: Delete projects deploy keys key.
      operationId: deleteV3ProjectsIdDeployKeysKeyId
      x-api-path-slug: v3projectsiddeploy-keyskey-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
  /v3/projects/{id}/deploy_keys/{key_id}/enable:
    post:
      summary: Post Projects Deploy Keys Key Enable
      description: This feature was added in GitLab 8.11
      operationId: postV3ProjectsIdDeployKeysKeyIdEnable
      x-api-path-slug: v3projectsiddeploy-keyskey-idenable-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
      - Enable
  /v3/projects/{id}/deploy_keys/{key_id}/disable:
    delete:
      summary: Delete Projects Deploy Keys Key Disable
      description: Delete projects deploy keys key disable.
      operationId: deleteV3ProjectsIdDeployKeysKeyIdDisable
      x-api-path-slug: v3projectsiddeploy-keyskey-iddisable-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
      - Disable
  /v3/deploy_keys:
    get:
      summary: Get Deploy Keys
      description: Get deploy keys.
      operationId: getV3DeployKeys
      x-api-path-slug: v3deploy-keys-get
      responses:
        200:
          description: OK
      tags:
      - Deploy
      - Keys
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