---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /applications/{application_id}/deployments.{format}:
    get:
      summary: Get Applications Application  Deployments. Format
      description: |-
        This API endpoint returns a paginated list of the deployments associated with a given application.

        See our documentation for a discussion on output pagination.
      operationId: getApplicationsApplicationDeployments.Format
      x-api-path-slug: applicationsapplication-iddeploymentsformat-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Deployments.
      - Format
    post:
      summary: Add Applications Application  Deployments. Format
      description: "This API endpoint creates a deployment record for a given application.\nDeployment
        records are created with the following attributes:\n\nRequired:\n\_\_- Application
        ID\n\_\_- Revision, such as a git SHA\n\nOptional:\n\_\_- Changelog \n\_\_-
        Description \n\_\_- User posting the deployment\n\nNote that the time of your
        deployment will be recorded as the current time in UTC."
      operationId: postApplicationsApplicationDeployments.Format
      x-api-path-slug: applicationsapplication-iddeploymentsformat-post
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: body
        name: deployment
        description: Deployment schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Deployments.
      - Format
  /applications/{application_id}/deployments/{id}.{format}:
    delete:
      summary: Delete Applications Application  Deployments  . Format
      description: "This API endpoint deletes the specified deployment record.\n\nNote:
        Admin User\u2019s API Key is required."
      operationId: deleteApplicationsApplicationDeployments.Format
      x-api-path-slug: applicationsapplication-iddeploymentsidformat-delete
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: path
        name: id
        description: Deployment ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Deployments
      - ""
      - .
      - Format
---