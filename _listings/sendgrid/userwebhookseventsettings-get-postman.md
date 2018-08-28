{
  "info": {
    "name": "SendGrid Get User Webhooks Event Settings",
    "_postman_id": "1f59eee0-12d7-4fc1-b449-bb3ca0a107d1",
    "description": "**This endpoint allows you to retrieve your current event webhook settings.**\n\nIf an event type is marked as `true`, then the event webhook will include information about that event.\n\nSendGrid???s Event Webhook will notify a URL of your choice via HTTP POST with information about events that occur as SendGrid processes your email.\n\nCommon uses of this data are to remove unsubscribes, react to spam reports, determine unengaged recipients, identify bounced email addresses, or create advanced analytics of your email program.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "79697c90-0f10-4213-ba1e-b9c04b1f4e10",
          "name": "user.webhooks.event.settings.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/user/webhooks/event/settings?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current event webhook settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "452dff28-db87-46b4-af6b-58dc1585a5e5"
            }
          ]
        }
      ]
    }
  ]
}