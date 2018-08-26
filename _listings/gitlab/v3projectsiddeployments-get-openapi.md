---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Deployments
  version: 1.0.0
  description: This feature was introduced in GitLab 8.11.
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