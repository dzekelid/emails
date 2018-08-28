{
  "info": {
    "name": "SendGrid Get Tracking Settings Subscription",
    "_postman_id": "daa8e759-62fd-463d-8b5f-12ea5e127595",
    "description": "**This endpoint allows you to retrieve your current settings for subscription tracking.**\n\nSubscription tracking adds links to the bottom of your emails that allows your recipients to subscribe to, or unsubscribe from, your emails.\n\nYou can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.\n\nFor more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "1c517b9a-613f-45c9-abb3-de6416f66d9e",
          "name": "tracking_settings.subscription.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/tracking_settings/subscription?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current settings for subscription tracking"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "524e923c-73ed-4c34-9796-8fa82e8bc3ff"
            }
          ]
        }
      ]
    }
  ]
}