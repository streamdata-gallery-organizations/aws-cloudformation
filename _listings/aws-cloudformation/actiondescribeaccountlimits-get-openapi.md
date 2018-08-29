---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 0
info:
  title: AWS CloudFormation API Describe Account Limits
  version: 1.0.0
  description: Retrieves your account's AWS CloudFormation limits, such as the maximum
    number of stacks that you can create in your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelUpdateStack:
    get:
      summary: Cancel Update Stack
      description: Cancels an update on the specified stack.
      operationId: cancelUpdateStack
      x-api-path-slug: actioncancelupdatestack-get
      parameters:
      - in: query
        name: StackName
        description: The name or the unique stack ID that is associated with the stack
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=ContinueUpdateRollback:
    get:
      summary: Continue Update Rollback
      description: |-
        For a specified stack that is in the UPDATE_ROLLBACK_FAILED state, continues rolling it back
                 to the UPDATE_ROLLBACK_COMPLETE state.
      operationId: continueUpdateRollback
      x-api-path-slug: actioncontinueupdaterollback-get
      parameters:
      - in: query
        name: ResourcesToSkip.member.N
        description: A list of the logical IDs of the resources that AWS CloudFormation
          skips during the continue update rollback operation
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to roll back
          the stack
        type: string
      - in: query
        name: StackName
        description: The name or the unique ID of the stack that you want to continue
          rolling back
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rollback
  /?Action=CreateChangeSet:
    get:
      summary: Create Change Set
      description: Creates a list of changes for a stack.
      operationId: createChangeSet
      x-api-path-slug: actioncreatechangeset-get
      parameters:
      - in: query
        name: Capabilities.member.N
        description: A list of values that you must specify before AWS CloudFormation
          can update certain stacks
        type: string
      - in: query
        name: ChangeSetName
        description: The name of the change set
        type: string
      - in: query
        name: ChangeSetType
        description: The type of change set operation
        type: string
      - in: query
        name: ClientToken
        description: A unique identifier for this CreateChangeSet request
        type: string
      - in: query
        name: Description
        description: A description to help you identify this change set
        type: string
      - in: query
        name: NotificationARNs.member.N
        description: The Amazon Resource Names (ARNs) of Amazon Simple Notification
          Service (Amazon SNS) topics that AWS CloudFormation associates with the
          stack
        type: string
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
          for the change set
        type: string
      - in: query
        name: ResourceTypes.member.N
        description: The template resource types that you have permissions to work
          with if you execute this change set, such as AWS::EC2::Instance, AWS::EC2::*,
          or Custom::MyCustomInstance
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes when executing
          the change set
        type: string
      - in: query
        name: StackName
        description: The name or the unique ID of the stack for which you are creating
          a change set
        type: string
      - in: query
        name: Tags.member.N
        description: Key-value pairs to associate with this stack
        type: string
      - in: query
        name: TemplateBody
        description: A structure that contains the body of the revised template, with
          a minimum length of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: The location of the file that contains the revised template
        type: string
      - in: query
        name: UsePreviousTemplate
        description: Whether to reuse the template that is associated with the stack
          to create the change set
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=CreateStack:
    get:
      summary: Create Stack
      description: Creates a stack as specified in the template.
      operationId: createStack
      x-api-path-slug: actioncreatestack-get
      parameters:
      - in: query
        name: Capabilities.member.N
        description: A list of values that you must specify before AWS CloudFormation
          can create certain stacks
        type: string
      - in: query
        name: DisableRollback
        description: Set to true to disable rollback of the stack if stack creation
          failed
        type: string
      - in: query
        name: NotificationARNs.member.N
        description: The Simple Notification Service (SNS) topic ARNs to publish stack
          related events
        type: string
      - in: query
        name: OnFailure
        description: Determines what action will be taken if stack creation fails
        type: string
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
          for the stack
        type: string
      - in: query
        name: ResourceTypes.member.N
        description: The template resource types that you have permissions to work
          with for this create stack action, such as AWS::EC2::Instance, AWS::EC2::*,
          or Custom::MyCustomInstance
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to create
          the stack
        type: string
      - in: query
        name: StackName
        description: The name that is associated with the stack
        type: string
      - in: query
        name: StackPolicyBody
        description: Structure containing the stack policy body
        type: string
      - in: query
        name: StackPolicyURL
        description: Location of a file containing the stack policy
        type: string
      - in: query
        name: Tags.member.N
        description: Key-value pairs to associate with this stack
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      - in: query
        name: TimeoutInMinutes
        description: The amount of time that can pass before the stack status becomes
          CREATE_FAILED; if DisableRollback         is not set or is set to false,
          the stack will be rolled back
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=DeleteChangeSet:
    get:
      summary: Delete Change Set
      description: Deletes the specified change set.
      operationId: deleteChangeSet
      x-api-path-slug: actiondeletechangeset-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of the change set that
          you want to delete
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set to delete, specify
          the stack name or ID (ARN) that is associated with it
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=DeleteStack:
    get:
      summary: Delete Stack
      description: Deletes a specified stack.
      operationId: deleteStack
      x-api-path-slug: actiondeletestack-get
      parameters:
      - in: query
        name: RetainResources.member.N
        description: For stacks in the DELETE_FAILED state, a list of resource logical
          IDs that are associated with          the resources you want to retain
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to delete
          the stack
        type: string
      - in: query
        name: StackName
        description: The name or the unique stack ID that is associated with the stack
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=DescribeAccountLimits:
    get:
      summary: Describe Account Limits
      description: Retrieves your account's AWS CloudFormation limits, such as the
        maximum number of stacks that you can create in your account.
      operationId: describeAccountLimits
      x-api-path-slug: actiondescribeaccountlimits-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of limits that you want
          to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Limits
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