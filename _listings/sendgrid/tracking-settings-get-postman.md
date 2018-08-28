{
  "info": {
    "name": "SendGrid Get Tracking Settings",
    "_postman_id": "795787da-aac8-4ffa-b854-966dcec0cdeb",
    "description": "**This endpoint allows you to retrieve a list of all tracking settings that you can enable on your account.**\n\nYou can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.\n\nFor more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "c03f8e18-b651-4b52-b3f5-cbf003b019aa",
          "name": "GET_tracking_settings",
          "request": {
            "url": "http://api.sendgrid.com/v3/tracking_settings?limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all tracking settings that you can enable on your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b50fa11e-c670-4134-835f-0d03b5e29a5d"
            }
          ]
        }
      ]
    }
  ]
}