---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update a variation bundle
  description: Updates a variation bundle component.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/{id}/variations/{variationId}/variation_bundles:
    get:
      summary: List bundle components
      description: List all components of a bundle. The ID of the item and the ID
        of the variation to which bundle components were added must be specified.
      operationId: getRestItemsVariationsVariationVariationBundles
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundles-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Bundle
      - Components
    post:
      summary: Add a variation to a bundle
      description: Adds a variation to a bundle variation as a bundle component.
      operationId: postRestItemsVariationsVariationVariationBundles
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundles-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_bundles
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - To
      - Bundle
  /rest/items/{id}/variations/{variationId}/variation_bundles/{bundleId}:
    delete:
      summary: Remove a bundle component
      description: Removes a component from a bundle. The bundle ID must be specified.
      operationId: deleteRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-delete
      parameters:
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Bundle
      - Component
    get:
      summary: Get a variation bundle
      description: Gets the bundle information for a specific bundle component.
      operationId: getRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-get
      parameters:
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Bundle
    put:
      summary: Update a variation bundle
      description: Updates a variation bundle component.
      operationId: putRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_bundles/{bundleId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Bundle
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