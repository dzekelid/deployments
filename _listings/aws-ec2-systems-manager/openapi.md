swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDeployablePatchSnapshotForInstance:
    get:
      summary: Get Deployable Patch Snapshot For Instance
      description: Retrieves the current snapshot for the patch baseline the instance
        uses.
      operationId: getDeployablePatchSnapshotForInstance
      x-api-path-slug: actiongetdeployablepatchsnapshotforinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance for which the appropriate patch snapshot
          should be retrieved
        type: string
      - in: query
        name: SnapshotId
        description: The user-defined snapshot ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployable
      - SnapshotInstance