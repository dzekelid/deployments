---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson Machine Learning Get Wml Instances Instance Published Models Published
    Model Deployments Deployment
  description: Get wml instances instance published models published model deployments
    deployment.
  version: 1.0.0
host: ibm-watson-ml.mybluemix.net
basePath: v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /wml_instances/{instance_id}/published_models/{published_model_id}/deployments:
    post:
      summary: Post Wml Instances Instance Published Models Published Model Deployments
      description: Creates the deployment - online, stream, batch (batch deployment
        only supports Cloud Object Storage as input/output for Tensorflow, Keras and
        Caffe models.)
      operationId: creates-the-deployment--online-stream-batch-batch-deployment-only-supports-cloud-object-storage-as-i
      x-api-path-slug: wml-instancesinstance-idpublished-modelspublished-model-iddeployments-post
      parameters:
      - in: body
        name: deployment_input
        description: The input data
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: sync
        description: This is parameter which determines if the online deployment needs
          to be created in synchronous or asynchronous way
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Wml
      - Instances
      - Instance
      - Id
      - Published
      - Models
      - Published
      - Model
      - Id
      - Deployments
    get:
      summary: Get Wml Instances Instance Published Models Published Model Deployments
      description: Get wml instances instance published models published model deployments.
      operationId: listDeploymentsForModel
      x-api-path-slug: wml-instancesinstance-idpublished-modelspublished-model-iddeployments-get
      parameters:
      - in: query
        name: status
        description: This is the filter parameter which allows to query deployments
          with the specific status
      - in: query
        name: type
        description: This is the filter parameter which allows to query deployments
          with the specific type
      - in: query
        name: _fields
        description: The list of fields which should be included in the response
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Wml
      - Instances
      - Instance
      - Id
      - Published
      - Models
      - Published
      - Model
      - Id
      - Deployments
  /wml_instances/{instance_id}/published_models/{published_model_id}/deployments/{deployment_id}:
    get:
      summary: Get Wml Instances Instance Published Models Published Model Deployments
        Deployment
      description: Get wml instances instance published models published model deployments
        deployment.
      operationId: getDeployment
      x-api-path-slug: wml-instancesinstance-idpublished-modelspublished-model-iddeploymentsdeployment-id-get
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Wml
      - Instances
      - Instance
      - Id
      - Published
      - Models
      - Published
      - Model
      - Id
      - Deployments
      - Deployment
      - Id
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