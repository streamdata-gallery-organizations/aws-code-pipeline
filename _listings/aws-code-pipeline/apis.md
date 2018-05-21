---
name: AWS Code Pipeline
x-slug: aws-code-pipeline
description: AWS Data Pipeline is a web service that helps you reliably process and
  move data between different AWS compute and storage services, as well as on-premise
  data sources, at specified intervals. With AWS Data Pipeline, you can regularly
  access your data where it&rsquo;s stored, transform and process it at scale, and
  efficiently transfer the results to AWS services such as Amazon S3, Amazon RDS,
  Amazon DynamoDB, and Amazon EMR.AWS Data Pipeline helps you easily create complex
  data processing workloads that are fault tolerant, repeatable, and highly available.
  You don&rsquo;t have to worry about ensuring resource availability, managing inter-task
  dependencies, retrying transient failures or timeouts in individual tasks, or creating
  a failure notification system. AWS Data Pipeline also allows you to move and process
  data that was previously locked up in on-premise data silos.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
x-kinRank: "10"
x-alexaRank: ""
tags: AWS Code Pipeline
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Code Pipeline API Acknowledge Job
  x-api-slug: aws-code-pipeline-api
  description: |-
    Returns information about a specified job and whether that job has been received by
                the job worker.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=AcknowledgeJob
  tags: Acknowledge, Job
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionacknowledgejob-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionacknowledgejob-get-openapi.md
- name: AWS Code Pipeline API Acknowledge Third Party Job
  x-api-slug: aws-code-pipeline-api
  description: Confirms a job worker has received the specified job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=AcknowledgeThirdPartyJob
  tags: Acknowledge, Third, Party, Job
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionacknowledgethirdpartyjob-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionacknowledgethirdpartyjob-get-openapi.md
- name: AWS Code Pipeline API Create Custom Action Type
  x-api-slug: aws-code-pipeline-api
  description: |-
    Creates a new custom action that can be used in all pipelines associated with the
                AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=CreateCustomActionType
  tags: Custom, Action, Type
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actioncreatecustomactiontype-get-openapi.md
- name: AWS Code Pipeline API Create Pipeline
  x-api-slug: aws-code-pipeline-api
  description: Creates a pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=CreatePipeline
  tags: Pipeline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actioncreatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actioncreatepipeline-get-openapi.md
- name: AWS Code Pipeline API Delete Custom Action Type
  x-api-slug: aws-code-pipeline-api
  description: Marks a custom action as deleted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=DeleteCustomActionType
  tags: Custom, Action, Type
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiondeletecustomactiontype-get-openapi.md
- name: AWS Code Pipeline API Delete Pipeline
  x-api-slug: aws-code-pipeline-api
  description: Deletes the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=DeletePipeline
  tags: Pipeline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiondeletepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiondeletepipeline-get-openapi.md
- name: AWS Code Pipeline API Disable Stage Transition
  x-api-slug: aws-code-pipeline-api
  description: |-
    Prevents artifacts in a pipeline from transitioning to the next stage in the
                pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=DisableStageTransition
  tags: Disable, Stage, Transition
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiondisablestagetransition-get-openapi.md
- name: AWS Code Pipeline API Enable Stage Transition
  x-api-slug: aws-code-pipeline-api
  description: Enables artifacts in a pipeline to transition to a stage in a pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=EnableStageTransition
  tags: Enable, Stage, Transition
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionenablestagetransition-get-openapi.md
- name: AWS Code Pipeline API Get Job Details
  x-api-slug: aws-code-pipeline-api
  description: Returns information about a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=GetJobDetails
  tags: Job, Details
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetjobdetails-get-openapi.md
- name: AWS Code Pipeline API Get Pipeline
  x-api-slug: aws-code-pipeline-api
  description: Returns the metadata, structure, stages, and actions of a pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=GetPipeline
  tags: Pipeline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetpipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetpipeline-get-openapi.md
- name: AWS Code Pipeline API Get Pipeline Execution
  x-api-slug: aws-code-pipeline-api
  description: |-
    Returns information about an execution of a pipeline, including details about
                artifacts, the pipeline execution ID, and the name, version, and status of the
                pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=GetPipelineExecution
  tags: Pipeline, Execution
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetpipelineexecution-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetpipelineexecution-get-openapi.md
- name: AWS Code Pipeline API Get Pipeline State
  x-api-slug: aws-code-pipeline-api
  description: |-
    Returns information about the state of a pipeline, including the stages and
                actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=GetPipelineState
  tags: Pipeline, State
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetpipelinestate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetpipelinestate-get-openapi.md
- name: AWS Code Pipeline API Get Third Party Job Details
  x-api-slug: aws-code-pipeline-api
  description: Requests the details of a job for a third party action.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=GetThirdPartyJobDetails
  tags: Third, Party, Job, Details
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actiongetthirdpartyjobdetails-get-openapi.md
- name: AWS Code Pipeline API List Action Types
  x-api-slug: aws-code-pipeline-api
  description: |-
    Gets a summary of all AWS CodePipeline action types associated with your
                account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=ListActionTypes
  tags: List, Action, Types
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionlistactiontypes-get-openapi.md
- name: AWS Code Pipeline API List Pipelines
  x-api-slug: aws-code-pipeline-api
  description: Gets a summary of all of the pipelines associated with your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=ListPipelines
  tags: List, Pipelines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionlistpipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionlistpipelines-get-openapi.md
- name: AWS Code Pipeline API Poll For Jobs
  x-api-slug: aws-code-pipeline-api
  description: Returns information about any jobs for AWS CodePipeline to act upon.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PollForJobs
  tags: PollJobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionpollforjobs-get-openapi.md
- name: AWS Code Pipeline API Poll For Third Party Jobs
  x-api-slug: aws-code-pipeline-api
  description: Determines whether there are any third party jobs for a job worker
    to act on.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PollForThirdPartyJobs
  tags: PollThird, Party, Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionpollforthirdpartyjobs-get-openapi.md
- name: AWS Code Pipeline API Put Action Revision
  x-api-slug: aws-code-pipeline-api
  description: Provides information to AWS CodePipeline about new revisions to a source.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PutActionRevision
  tags: Put, Action, Revision
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputactionrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputactionrevision-get-openapi.md
- name: AWS Code Pipeline API Put Approval Result
  x-api-slug: aws-code-pipeline-api
  description: Provides the response to a manual approval request to AWS CodePipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PutApprovalResult
  tags: Put, Approval, Result
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputapprovalresult-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputapprovalresult-get-openapi.md
- name: AWS Code Pipeline API Put Job Failure Result
  x-api-slug: aws-code-pipeline-api
  description: Represents the failure of a job as returned to the pipeline by a job
    worker.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PutJobFailureResult
  tags: Put, Job, Failure, Result
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputjobfailureresult-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputjobfailureresult-get-openapi.md
- name: AWS Code Pipeline API Put Job Success Result
  x-api-slug: aws-code-pipeline-api
  description: Represents the success of a job as returned to the pipeline by a job
    worker.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PutJobSuccessResult
  tags: Put, Job, Success, Result
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputjobsuccessresult-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputjobsuccessresult-get-openapi.md
- name: AWS Code Pipeline API Put Third Party Job Failure Result
  x-api-slug: aws-code-pipeline-api
  description: |-
    Represents the failure of a third party job as returned to the pipeline by a job
                worker.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PutThirdPartyJobFailureResult
  tags: Put, Third, Party, Job, Failure, Result
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputthirdpartyjobfailureresult-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputthirdpartyjobfailureresult-get-openapi.md
- name: AWS Code Pipeline API Put Third Party Job Success Result
  x-api-slug: aws-code-pipeline-api
  description: |-
    Represents the success of a third party job as returned to the pipeline by a job
                worker.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PutThirdPartyJobSuccessResult
  tags: Put, Third, Party, Job, Success, Result
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputthirdpartyjobsuccessresult-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionputthirdpartyjobsuccessresult-get-openapi.md
- name: AWS Code Pipeline API Retry Stage Execution
  x-api-slug: aws-code-pipeline-api
  description: |-
    Resumes the pipeline execution by retrying the last failed actions in a
                stage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=RetryStageExecution
  tags: Retry, Stage, Execution
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionretrystageexecution-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionretrystageexecution-get-openapi.md
- name: AWS Code Pipeline API Start Pipeline Execution
  x-api-slug: aws-code-pipeline-api
  description: Starts the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=StartPipelineExecution
  tags: Start, Pipeline, Execution
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionstartpipelineexecution-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionstartpipelineexecution-get-openapi.md
- name: AWS Code Pipeline API Update Pipeline
  x-api-slug: aws-code-pipeline-api
  description: Updates a specified pipeline with edits or changes to its structure.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=UpdatePipeline
  tags: Pipeline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionupdatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/actionupdatepipeline-get-openapi.md
- name: AWS Code Pipeline API
  x-api-slug: aws-code-pipeline-api
  description: AWS Data Pipeline is a web service that helps you reliably process
    and move data between different AWS compute and storage services, as well as on-premise
    data sources, at specified intervals. With AWS Data Pipeline, you can regularly
    access your data where it&rsquo;s stored, transform and process it at scale, and
    efficiently transfer the results to AWS services such as Amazon S3, Amazon RDS,
    Amazon DynamoDB, and Amazon EMR.AWS Data Pipeline helps you easily create complex
    data processing workloads that are fault tolerant, repeatable, and highly available.
    You don&rsquo;t have to worry about ensuring resource availability, managing inter-task
    dependencies, retrying transient failures or timeouts in individual tasks, or
    creating a failure notification system. AWS Data Pipeline also allows you to move
    and process data that was previously locked up in on-premise data silos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Developer-Tools_AWSCodePipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: AWS Code Pipeline
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-code-pipeline/master/_listings/aws-code-pipeline/openapi.md
x-common:
- type: x-blog
  url: http://blogs.aws.amazon.com/bigdata
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/AWS-Data-Pipeline/
- type: x-documentation
  url: http://docs.aws.amazon.com/datapipeline/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/datapipeline/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=151
- type: x-pricing
  url: https://aws.amazon.com/datapipeline/pricing/
- type: x-tools
  url: http://aws.amazon.com/developertools/AWS-Data-Pipeline/
- type: x-website
  url: https://aws.amazon.com/datapipeline/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---