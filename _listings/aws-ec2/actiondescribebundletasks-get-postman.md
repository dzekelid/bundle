{
  "info": {
    "name": "AWS EC2 API Describe Bundle Tasks",
    "_postman_id": "0028ab55-6fbe-4dc4-b260-8906b9b938de",
    "description": "Describes one or more of your bundling tasks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bundle Task",
      "item": [
        {
          "id": "52e6cb6d-e47e-4a2d-bbb0-d880b3f4f45a",
          "name": "cancelbundletask",
          "request": {
            "url": "http://example.com/api/?Action=CancelBundleTask?BundleId.N=BundleId.N&DryRun=DryRun&Filter.N=Filter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a bundling operation for an instance store-backed Windows instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "059daa10-abcc-4372-b8a9-b6893b252b81"
            }
          ]
        },
        {
          "id": "435359c4-1861-456b-897a-3132b63c0151",
          "name": "describebundletasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeBundleTasks?DryRun=DryRun&InstanceId=InstanceId&SecurityGroupId.N=SecurityGroupId.N&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your bundling tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dbacee3-2de7-4547-992e-5e75ae23bd33"
            }
          ]
        }
      ]
    }
  ]
}