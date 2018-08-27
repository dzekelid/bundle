swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BundleInstance:
    get:
      summary: Bundle Instance
      description: Bundles an Amazon instance store-backed Windows instance.
      operationId: bundleinstance
      x-api-path-slug: actionbundleinstance-get
      parameters:
      - in: query
        name: BundleId
        description: The ID of the bundle task
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundle Instance
  /?Action=CancelBundleTask:
    get:
      summary: Cancel Bundle Task
      description: Cancels a bundling operation for an instance store-backed Windows
        instance.
      operationId: cancelbundletask
      x-api-path-slug: actioncancelbundletask-get
      parameters:
      - in: query
        name: BundleId.N
        description: One or more bundle task IDs
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundle Task
  /?Action=DescribeBundleTasks:
    get:
      summary: Describe Bundle Tasks
      description: Describes one or more of your bundling tasks.
      operationId: describebundletasks
      x-api-path-slug: actiondescribebundletasks-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of an EC2-Classic instance to link to the ClassicLink-enabled
          VPC
        type: string
      - in: query
        name: SecurityGroupId.N
        description: The ID of one or more of the VPCs security groups
        type: string
      - in: query
        name: VpcId
        description: The ID of a ClassicLink-enabled VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundle Task