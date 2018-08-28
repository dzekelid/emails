{
  "info": {
    "name": "SendGrid Get Tracking Settings Click",
    "_postman_id": "aac07d14-9ec3-45a9-b28b-8faf54440c34",
    "description": "**This endpoint allows you to retrieve your current click tracking setting.**\n\nYou can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.\n\nFor more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "7ca18890-978f-44bf-b14b-9c447d795818",
          "name": "tracking_settings.click.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/tracking_settings/click?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current click tracking setting"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "100fefaf-f149-416f-afc1-da981723ff0a"
            }
          ]
        }
      ]
    }
  ]
}