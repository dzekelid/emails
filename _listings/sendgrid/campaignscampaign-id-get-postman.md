{
  "info": {
    "name": "SendGrid Get Campaigns Campaign",
    "_postman_id": "123ae72e-4f7e-4913-a276-af8a064fdd7b",
    "description": "**This endpoint allows you to retrieve a specific campaign.**\n\nOur Marketing Campaigns API lets you create, manage, send, and schedule campaigns.\n\nFor more information:\n\n* [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "6916afb6-4a58-4c32-9ecb-8743a73e33a3",
          "name": "campaigns.campaign_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "campaigns/:campaign_id"
              ],
              "variable": [
                {
                  "id": "campaign_id",
                  "value": "campaign_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a specific campaign"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a496a6e-fd0e-4c48-ab4f-aeae876c8d32"
            }
          ]
        }
      ]
    }
  ]
}