---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Post Deployments
  description: Creates a new deployment. It requires any project role, or the **administrator**
    or **project creator** global role.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deployments:
    get:
      summary: Get Deployments
      description: Returns deployments. It requires any project role or non-'consumer'
        global role.
      operationId: FindDeployments
      x-api-path-slug: deployments-get
      parameters:
      - in: query
        name: query
        description: Filters the deployments returned
      - in: query
        name: userQuery
        description: Filters the deployments returned
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include zone, service,
          volume details'
      responses:
        200:
          description: OK
      tags:
      - Deployments
    post:
      summary: Post Deployments
      description: Creates a new deployment. It requires any project role, or the
        **administrator** or **project creator** global role.
      operationId: CreateDeployment
      x-api-path-slug: deployments-post
      parameters:
      - in: body
        name: deployment
        description: Add new deployment
        schema:
          $ref: '#/definitions/holder'
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