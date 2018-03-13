---
swagger: "2.0"
info:
  title: APImetrics Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deployments/call/{call_id}/:
    get:
      summary: Get all Deployments for an API Call
      description: Get all Deployments for an API Call
      operationId: getAllDeploymentForAPICall
      parameters:
      - in: path
        name: call_id
        description: ID of the API Call
      responses:
        200:
          description: OK
      tags:
      - monitoring
      - deployments
      - call
      - call
definitions: []
x-collection-name: APImetrics
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