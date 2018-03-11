---
swagger: "2.0"
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ExecuteChangeSet&k=1:
    get:
      summary: ' Execute Change Set '
      description: Updates a stack using the input information that was provided when
        the specified change set was created
      operationId: executeChangeSet
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or ARN of the change set that you want use to update
          the specified stack
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set, specify the stack
          name or ID (ARN) that is associated with the change set you want to execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - change sets
definitions: []
x-collection-name: AWS CloudFormation
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