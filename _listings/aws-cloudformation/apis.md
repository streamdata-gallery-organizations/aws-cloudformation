---
name: AWS CloudFormation
x-slug: aws-cloudformation
description: AWS CloudFormation gives developers and systems administrators an easy
  way to create and manage a collection of related AWS resources, provisioning and
  updating them in an orderly and predictable fashion.You can use AWS CloudFormations?sample
  templates?or create your own templates to describe the AWS resources, and any associated
  dependencies or runtime parameters, required to run your application. You do not
  need to figure out the order for provisioning AWS services or the subtleties of
  making those dependencies work. CloudFormation takes care of this for you. After
  the AWS resources are deployed, you can modify and update them in a controlled and
  predictable way, in effect applying version control to your AWS infrastructure the
  same way you do with your software. You can also visualize your templates as diagrams
  and edit them using a drag-and-drop interface with the?AWS CloudFormation Designer.You
  can deploy and update a template and its associated collection of resources (called
  a stack) by using the AWS Management Console, AWS Command Line Interface, or APIs.
  CloudFormation is available at no additional charge, and you pay only for the AWS
  resources needed to run your applications.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
x-kinRank: "10"
x-alexaRank: "0"
tags: AWS CloudFormation
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/apis.md
specificationVersion: "0.14"
apis:
- name: AWS CloudFormation API Cancel Update Stack
  x-api-slug: aws-cloudformation-api
  description: Cancels an update on the specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=CancelUpdateStack
  tags: Stacks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncancelupdatestack-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncancelupdatestack-get-openapi.md
- name: AWS CloudFormation API Continue Update Rollback
  x-api-slug: aws-cloudformation-api
  description: |-
    For a specified stack that is in the UPDATE_ROLLBACK_FAILED state, continues rolling it back
             to the UPDATE_ROLLBACK_COMPLETE state.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ContinueUpdateRollback
  tags: Rollback
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncontinueupdaterollback-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncontinueupdaterollback-get-openapi.md
- name: AWS CloudFormation API Create Change Set
  x-api-slug: aws-cloudformation-api
  description: Creates a list of changes for a stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=CreateChangeSet
  tags: Change Sets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncreatechangeset-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncreatechangeset-get-openapi.md
- name: AWS CloudFormation API Create Stack
  x-api-slug: aws-cloudformation-api
  description: Creates a stack as specified in the template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=CreateStack
  tags: Stacks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncreatestack-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actioncreatestack-get-openapi.md
- name: AWS CloudFormation API Delete Change Set
  x-api-slug: aws-cloudformation-api
  description: Deletes the specified change set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DeleteChangeSet
  tags: Change Sets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondeletechangeset-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondeletechangeset-get-openapi.md
- name: AWS CloudFormation API Delete Stack
  x-api-slug: aws-cloudformation-api
  description: Deletes a specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DeleteStack
  tags: Stacks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondeletestack-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondeletestack-get-openapi.md
- name: AWS CloudFormation API Describe Account Limits
  x-api-slug: aws-cloudformation-api
  description: Retrieves your account's AWS CloudFormation limits, such as the maximum
    number of stacks that you can create in your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DescribeAccountLimits
  tags: Account Limits
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribeaccountlimits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribeaccountlimits-get-openapi.md
- name: AWS CloudFormation API Describe Change Set
  x-api-slug: aws-cloudformation-api
  description: Returns the inputs for the change set and a list of changes that AWS
    CloudFormation will make if you execute the change set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DescribeChangeSet
  tags: Change Sets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribechangeset-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribechangeset-get-openapi.md
- name: AWS CloudFormation API Describe Stack Events
  x-api-slug: aws-cloudformation-api
  description: Returns all stack related events for a specified stack in reverse chronological
    order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DescribeStackEvents
  tags: Stack Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribestackevents-get-openapi.md
- name: AWS CloudFormation API Describe Stack Resource
  x-api-slug: aws-cloudformation-api
  description: Returns a description of the specified resource in the specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DescribeStackResource
  tags: Stack Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribestackresource-get-openapi.md
- name: AWS CloudFormation API Describe Stack Resources
  x-api-slug: aws-cloudformation-api
  description: Returns AWS resource descriptions for running and deleted stacks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DescribeStackResources
  tags: Stack Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribestackresources-get-openapi.md
- name: AWS CloudFormation API Describe Stacks
  x-api-slug: aws-cloudformation-api
  description: Returns the description for the specified stack; if no stack name was
    specified, then it returns the description for all the stacks created.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=DescribeStacks
  tags: Stacks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribestacks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiondescribestacks-get-openapi.md
- name: AWS CloudFormation API Estimate Template Cost
  x-api-slug: aws-cloudformation-api
  description: Returns the estimated monthly cost of a template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=EstimateTemplateCost
  tags: Template Cost
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionestimatetemplatecost-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionestimatetemplatecost-get-openapi.md
- name: AWS CloudFormation API Execute Change Set
  x-api-slug: aws-cloudformation-api
  description: Updates a stack using the input information that was provided when
    the specified change set was created.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ExecuteChangeSet
  tags: Change Sets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionexecutechangeset-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionexecutechangeset-get-openapi.md
- name: AWS CloudFormation API Get Stack Policy
  x-api-slug: aws-cloudformation-api
  description: Returns the stack policy for a specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=GetStackPolicy
  tags: Stack Policies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiongetstackpolicy-get-openapi.md
- name: AWS CloudFormation API Get Template
  x-api-slug: aws-cloudformation-api
  description: Returns the template body for a specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=GetTemplate
  tags: Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiongettemplate-get-openapi.md
- name: AWS CloudFormation API Get Template Summary
  x-api-slug: aws-cloudformation-api
  description: Returns information about a new or existing template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=GetTemplateSummary
  tags: Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actiongettemplatesummary-get-openapi.md
- name: AWS CloudFormation API List Change Sets
  x-api-slug: aws-cloudformation-api
  description: Returns the ID and status of each active change set for a stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ListChangeSets
  tags: Change Sets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionlistchangesets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionlistchangesets-get-openapi.md
- name: AWS CloudFormation API List Exports
  x-api-slug: aws-cloudformation-api
  description: Lists all exported output values in the account and region in which
    you call this action.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ListExports
  tags: Exports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionlistexports-get-openapi.md
- name: AWS CloudFormation API List Imports
  x-api-slug: aws-cloudformation-api
  description: Lists all stacks that are importing an exported output value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ListImports
  tags: Imports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionlistimports-get-openapi.md
- name: AWS CloudFormation API List Stack Resources
  x-api-slug: aws-cloudformation-api
  description: Returns descriptions of all resources of the specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ListStackResources
  tags: Stack Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionliststackresources-get-openapi.md
- name: AWS CloudFormation API List Stacks
  x-api-slug: aws-cloudformation-api
  description: Returns the summary information for stacks whose status matches the
    specified StackStatusFilter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ListStacks
  tags: Stacks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionliststacks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionliststacks-get-openapi.md
- name: AWS CloudFormation API Set Stack Policy
  x-api-slug: aws-cloudformation-api
  description: Sets a stack policy for a specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=SetStackPolicy
  tags: Stack Policies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionsetstackpolicy-get-openapi.md
- name: AWS CloudFormation API Signal Resource
  x-api-slug: aws-cloudformation-api
  description: Sends a signal to the specified resource with a success or failure
    status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=SignalResource
  tags: Signal Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionsignalresource-get-openapi.md
- name: AWS CloudFormation API Update Stack
  x-api-slug: aws-cloudformation-api
  description: Updates a stack as specified in the template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=UpdateStack
  tags: Stacks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionupdatestack-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionupdatestack-get-openapi.md
- name: AWS CloudFormation API Validate Template
  x-api-slug: aws-cloudformation-api
  description: Validates a specified template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: ://///?Action=ValidateTemplate
  tags: Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/actionvalidatetemplate-get-openapi.md
- name: AWS CloudFormation API
  x-api-slug: aws-cloudformation-api
  description: AWS CloudFormation gives developers and systems administrators an easy
    way to create and manage a collection of related AWS resources, provisioning and
    updating them in an orderly and predictable fashion.You can use AWS CloudFormations?sample
    templates?or create your own templates to describe the AWS resources, and any
    associated dependencies or runtime parameters, required to run your application.
    You do not need to figure out the order for provisioning AWS services or the subtleties
    of making those dependencies work. CloudFormation takes care of this for you.
    After the AWS resources are deployed, you can modify and update them in a controlled
    and predictable way, in effect applying version control to your AWS infrastructure
    the same way you do with your software. You can also visualize your templates
    as diagrams and edit them using a drag-and-drop interface with the?AWS CloudFormation
    Designer.You can deploy and update a template and its associated collection of
    resources (called a stack) by using the AWS Management Console, AWS Command Line
    Interface, or APIs. CloudFormation is available at no additional charge, and you
    pay only for the AWS resources needed to run your applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudFormation.png
  humanURL: https://aws.amazon.com/cloudformation/
  baseURL: :///
  tags: AWS CloudFormation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudformation/master/_listings/aws-cloudformation/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/cloudformation/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/cloudformation/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/cloudformation/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/cloudformation/pricing/
- type: x-sdk
  url: https://aws.amazon.com/cloudformation/aws-cloudformation-templates/
- type: x-website
  url: https://aws.amazon.com/cloudformation/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---