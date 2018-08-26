---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetBundles:
    get:
      summary: Get Bundles
      description: Returns the list of bundles that are available for purchase.
      operationId: getBundles
      x-api-path-slug: actiongetbundles-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value that indicates whether to include inactive bundle
          results in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get bundles      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundles
---