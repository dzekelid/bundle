---
swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 1
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
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
---