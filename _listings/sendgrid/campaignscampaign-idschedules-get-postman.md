{
  "info": {
    "name": "SendGrid Get Campaigns Campaign  Schedules",
    "_postman_id": "d2d9a47d-3336-4236-8334-f837810c5b60",
    "description": "**This endpoint allows you to retrieve the date and time that the given campaign has been scheduled to be sent.**\n\nFor more information:\n\n* [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "29e4095d-f245-4f5f-9001-00d6567f4683",
          "name": "campaigns.campaign_id.schedules.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "campaigns/:campaign_id/schedules"
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
            "description": "**This endpoint allows you to retrieve the date and time that the given campaign has been scheduled to be sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45d1c92e-88b4-4188-83bd-625e71770b45"
            }
          ]
        }
      ]
    }
  ]
}