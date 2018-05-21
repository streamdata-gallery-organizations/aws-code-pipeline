---
swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 0
info:
  title: AWS Code Pipeline API Get Job Details
  version: 1.0.0
  description: Returns information about a job.
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
  /?Action=CreateCustomActionType:
    get:
      summary: Create Custom Action Type
      description: |-
        Creates a new custom action that can be used in all pipelines associated with the
                    AWS account.
      operationId: createCustomActionType
      x-api-path-slug: actioncreatecustomactiontype-get
      parameters:
      - in: query
        name: Attribute
        description: The snapshot attribute you would like to view
        type: string
      - in: query
        name: category
        description: The category of the custom action, such as a build action or
          a test            action
        type: string
      - in: query
        name: configurationProperties
        description: The configuration properties for the custom action
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: inputArtifactDetails
        description: Returns information about the details of an artifact
        type: string
      - in: query
        name: outputArtifactDetails
        description: Returns information about the details of an artifact
        type: string
      - in: query
        name: provider
        description: The provider of the service used in the custom action, such as
          AWS            CodeDeploy
        type: string
      - in: query
        name: settings
        description: Returns information about the settings for an action type
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the EBS snapshot
        type: string
      - in: query
        name: version
        description: The version identifier of the custom action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Action
      - Type
  /?Action=CreatePipeline:
    get:
      summary: Create Pipeline
      description: Creates a pipeline.
      operationId: createPipeline
      x-api-path-slug: actioncreatepipeline-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of snapshot results returned by DescribeSnapshots
          in      paginated output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeSnapshots
          request where MaxResults was used and the      results exceeded the value
          of that parameter
        type: string
      - in: query
        name: Owner.N
        description: Returns the snapshots owned by the specified owner
        type: string
      - in: query
        name: pipeline
        description: Represents the structure of actions and stages to be performed
          in the            pipeline
        type: string
      - in: query
        name: RestorableBy.N
        description: One or more AWS accounts IDs that can create volumes from the
          snapshot
        type: string
      - in: query
        name: SnapshotId.N
        description: One or more snapshot IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DeleteCustomActionType:
    get:
      summary: Delete Custom Action Type
      description: Marks a custom action as deleted.
      operationId: deleteCustomActionType
      x-api-path-slug: actiondeletecustomactiontype-get
      parameters:
      - in: query
        name: Attribute
        description: The instance attribute
        type: string
      - in: query
        name: category
        description: The category of the custom action that you want to delete, such
          as source or            deploy
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: provider
        description: The provider of the service used in the custom action, such as
          AWS            CodeDeploy
        type: string
      - in: query
        name: version
        description: The version of the custom action to delete
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Action
      - Type
  /?Action=DeletePipeline:
    get:
      summary: Delete Pipeline
      description: Deletes the specified pipeline.
      operationId: deletePipeline
      x-api-path-slug: actiondeletepipeline-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of volume results returned by DescribeVolumes
          in paginated      output
        type: string
      - in: query
        name: name
        description: The name of the pipeline to be deleted
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeVolumes
          request where MaxResults was used and the results      exceeded the value
          of that parameter
        type: string
      - in: query
        name: VolumeId.N
        description: One or more volume IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DisableStageTransition:
    get:
      summary: Disable Stage Transition
      description: |-
        Prevents artifacts in a pipeline from transitioning to the next stage in the
                    pipeline.
      operationId: disableStageTransition
      x-api-path-slug: actiondisablestagetransition-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of volume results returned by DescribeVolumeStatus
          in      paginated output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value to include in a future DescribeVolumeStatus      request
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline in which you want to disable the flow
          of artifacts from            one stage to another
        type: string
      - in: query
        name: reason
        description: The reason given to the user why a stage is disabled, such as
          waiting for manual            approval or manual tests
        type: string
      - in: query
        name: stageName
        description: The name of the stage where you want to disable the inbound or
          outbound transition            of artifacts
        type: string
      - in: query
        name: transitionType
        description: Specifies whether artifacts will be prevented from transitioning
          into the stage and            being processed by the actions in that stage
          (inbound), or prevented from transitioning            from the stage after
          they have been processed by the actions in that stage            (outbound)
        type: string
      - in: query
        name: VolumeId.N
        description: One or more volume IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Disable
      - Stage
      - Transition
  /?Action=EnableStageTransition:
    get:
      summary: Enable Stage Transition
      description: Enables artifacts in a pipeline to transition to a stage in a pipeline.
      operationId: enableStageTransition
      x-api-path-slug: actionenablestagetransition-get
      parameters:
      - in: query
        name: Device
        description: The device name
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Force
        description: Forces detachment if the previous detachment attempt did not
          occur cleanly (for example,      logging into an instance, unmounting the
          volume, and detaching normally)
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline in which you want to enable the flow
          of artifacts from one            stage to another
        type: string
      - in: query
        name: stageName
        description: The name of the stage where you want to enable the transition
          of artifacts, either            into the stage (inbound) or from that stage
          to the next stage (outbound)
        type: string
      - in: query
        name: transitionType
        description: Specifies whether artifacts will be allowed to enter the stage
          and be processed by            the actions in that stage (inbound) or whether
          already-processed artifacts will be            allowed to transition to
          the next stage (outbound)
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Enable
      - Stage
      - Transition
  /?Action=GetJobDetails:
    get:
      summary: Get Job Details
      description: Returns information about a job.
      operationId: getJobDetails
      x-api-path-slug: actiongetjobdetails-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID for the job
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job
      - Details
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