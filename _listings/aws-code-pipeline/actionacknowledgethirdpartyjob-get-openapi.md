---
swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 0
info:
  title: AWS Code Pipeline API Acknowledge Third Party Job
  version: 1.0.0
  description: Confirms a job worker has received the specified job.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcknowledgeJob:
    get:
      summary: Acknowledge Job
      description: |-
        Returns information about a specified job and whether that job has been received by
                    the job worker.
      operationId: acknowledgeJob
      x-api-path-slug: actionacknowledgejob-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job for which you want
          to confirm            receipt
        type: string
      - in: query
        name: nonce
        description: A system-generated random number that AWS CodePipeline uses to
          ensure that the job            is being worked on by only one job worker
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the EBS snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Job
  /?Action=AcknowledgeThirdPartyJob:
    get:
      summary: Acknowledge Third Party Job
      description: Confirms a job worker has received the specified job.
      operationId: acknowledgeThirdPartyJob
      x-api-path-slug: actionacknowledgethirdpartyjob-get
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job
        type: string
      - in: query
        name: nonce
        description: A system-generated random number that AWS CodePipeline uses to
          ensure that the job            is being worked on by only one job worker
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Third
      - Party
      - Job
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