---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Listings Listing Product Bundle
  description: Find a product bundle attached to a listing
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listings/{listing_id}/product_bundle:
    get:
      summary: Get Listings Listing Product Bundle
      description: Find a product bundle attached to a listing
      operationId: getListingsListingProductBundle
      x-api-path-slug: listingslisting-idproduct-bundle-get
      parameters:
      - in: query
        name: for_seller
        description: Pass to see non-live bundles as the seller
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Product
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