---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 0
info:
  title: AWS CloudFormation API Create Change Set
  version: 1.0.0
  description: Creates a list of changes for a stack.
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