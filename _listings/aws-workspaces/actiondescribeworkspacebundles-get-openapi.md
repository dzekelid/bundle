---
swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 0
info:
  title: AWS WorkSpaces Service API Describe Workspace Bundles
  version: 1.0.0
  description: Obtains information about the WorkSpace bundles that are available
    to your account in the specified region.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeWorkspaceBundles:
    get:
      summary: Describe Workspace Bundles
      description: Obtains information about the WorkSpace bundles that are available
        to your account in the specified region.
      operationId: describeWorkspaceBundles
      x-api-path-slug: actiondescribeworkspacebundles-get
      parameters:
      - in: query
        name: BundleIds
        description: An array of strings that contains the identifiers of the bundles
          to retrieve
        type: string
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to this operation
        type: string
      - in: query
        name: Owner
        description: The owner of the bundles to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspace Bundles
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