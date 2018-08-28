{
  "info": {
    "name": "SendGrid Get Tracking Settings Open",
    "_postman_id": "1d533975-1c02-454c-a790-ca4a6295e452",
    "description": "**This endpoint allows you to retrieve your current settings for open tracking.**\n\nOpen Tracking adds an invisible image at the end of the email which can track email opens. If the email recipient has images enabled on their email client, a request to SendGrid???s server for the invisible image is executed and an open event is logged. These events are logged in the Statistics portal, Email Activity interface, and are reported by the Event Webhook.\n\nYou can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.\n\nFor more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "c44500f8-5125-458c-9d17-df03d93b7c6f",
          "name": "tracking_settings.open.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/tracking_settings/open?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current settings for open tracking"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72a9f05a-752d-47be-82b8-be0265a4924f"
            }
          ]
        }
      ]
    }
  ]
}