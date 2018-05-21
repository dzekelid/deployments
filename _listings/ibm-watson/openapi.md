---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 1
info:
  title: IBM Watson Machine Learning API
  description: -authorizationstep-by-step-instruction-how-to-use-watson-machine-learning-servicecan-be-found-herehttpsdatascienceibmcomdocscontentanalyzedatamloverviewhtmlcontextanalytics-ibm-watson-machine-learning-credentialsto-start-working-with-api-one-needs-to-generate-an-access-token-using-the-username-and-passwordavailable-on-the-service-credentials-tab-of-the-ibm-watson-machine-learning-service-instance-or-also-available-in-the-vcap-environment-variableexample-of-the-service-credentialsjson----url-httpsibmwatsonmlmybluemixnet----username-c1ef4b802ee2458eab92e9ca97ec657d----password-030528d45a3e4d4c92585d553513be6f----instance-id-a751c209954edc32b441ad56ce7a9f40example-of-obtaining-access-token-from-token-endpoint-using-http-basic-auth-for-details-please-refer-to-token-section-belowcurl-basic-user-usernamepassword-httpsibmwatsonmlmybluemixnetv3identitytokenthe-obtained-access-token-needs-to-be-prepended-with-bearer-word-and-it-needs-to-be-passed-in-the-authorization-header-for-api-callsexample-of-api-request-with-bearer-access-tokencurl-httpsibmwatsonmlmybluemixnetv3wml-instances00fd89e68cf24712a068ade10277b649published-models-h-authorization-bearer-eyjhbgcioijsuzuxmiisinr5cci6ikpxvcj9eyj0zw5hbnrjzci6imu4ymqzzgm3lwi5y2utndy1oc1iz-apache-spark-service-credentialsthe-ibm-watson-machine-learning-cooperates-with-the-apache-spark-as-a-service-to-create-batch-stream-deploymentsand-for-learning-configuration-functionalityfor-api-methods-requiring-apache-spark-service-instance-a-custom-header-xsparkserviceinstancewith-service-credentials-must-be-specifiedthe-header-value-is-a-base64-encoded-string-with-the-json-data-containing-service-credentials-and-spark-versionexample-of-the-json-data---credentials------tenant-ids068ade10277b6495605b1d10fv12b------tenant-id-full00fd89e68cf24712a068ade10277b649-41f37bf21b954c65a15605b1d10fb12b------cluster-master-urlhttpssparkbluemixnet------instance-id00fd89e68cf24712a068ade10277b649------tenant-secretc74c37cf482a4da4836ef32ca26ccbb9------planibmsparkservicepaygopersonal------version20
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
    patch:
      summary: Patch Wml Instances Instance Published Models Published Model Deployments
        Deployment
      description: Patch wml instances instance published models published model deployments
        deployment.
      operationId: allows-to-update-the-deployed-stream-status-startstop
      x-api-path-slug: wml-instancesinstance-idpublished-modelspublished-model-iddeploymentsdeployment-id-patch
      parameters:
      - in: body
        name: deployment_patch
        description: Input For Patch
        schema:
          $ref: '#/definitions/holder'
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
    delete:
      summary: Delete Wml Instances Instance Published Models Published Model Deployments
        Deployment
      description: Delete wml instances instance published models published model
        deployments deployment.
      operationId: ""
      x-api-path-slug: wml-instancesinstance-idpublished-modelspublished-model-iddeploymentsdeployment-id-delete
      parameters:
      - in: query
        name: ignore_spark_errors
        description: If this flag is set to true then the deployment will be deleted
          even if spark reports failure in response to kill job request
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
  /wml_instances/{instance_id}/published_models/{published_model_id}/deployments/{deployment_id}/online:
    post:
      summary: Post Wml Instances Instance Published Models Published Model Deployments
        Deployment Online
      description: Post wml instances instance published models published model deployments
        deployment online.
      operationId: makes-an-online-prediction-on-a-given-data-values
      x-api-path-slug: wml-instancesinstance-idpublished-modelspublished-model-iddeploymentsdeployment-idonline-post
      parameters:
      - in: body
        name: online_prediction_input
        description: The input data
        schema:
          $ref: '#/definitions/holder'
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
      - Online
  /wml_instances/{instance_id}/deployments:
    get:
      summary: Get Wml Instances Instance Deployments
      description: Get wml instances instance deployments.
      operationId: listAllDeployments
      x-api-path-slug: wml-instancesinstance-iddeployments-get
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Wml
      - Instances
      - Instance
      - Id
      - Deployments
---