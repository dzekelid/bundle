{
  "info": {
    "name": "Plentymarkets List bundle components",
    "_postman_id": "1349d71f-f6ba-4d6f-a601-7ce72a69bf4c",
    "description": "List all components of a bundle. The ID of the item and the ID of the variation to which bundle components were added must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "4f9923e9-f22a-4a4f-98bf-1098dc92550c",
          "name": "getRestItemsVariationsVariationVariationBundles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_bundles"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List all components of a bundle. The ID of the item and the ID of the variation to which bundle components were added must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c52ea3e-4939-4a21-9722-089bb00ac0a5"
            }
          ]
        }
      ]
    }
  ]
}