---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cps/v2/enrollments/{enrollmentId}/deployments/production:
    get:
      summary: Get a Certificate
      description: Get a Certificate
      operationId: cpsv2enrollmentsenrollmentiddeploymentsproduction
      x-api-path-slug: cpsv2enrollmentsenrollmentiddeploymentsproduction-get
      parameters:
      - in: query
        name: enrollmentId
        description: Unique integer identifer for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Deployments
      - Production
---