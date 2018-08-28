{
  "info": {
    "name": "SendGrid Get Mail Settings Forward Bounce",
    "_postman_id": "75f059e4-116c-4629-8012-fca6b071b5db",
    "description": "**This endpoint allows you to retrieve your current bounce forwarding mail settings.**\n\nActivating this setting allows you to specify an email address to which bounce reports are forwarded.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "ebdb76c5-2f7b-4881-b735-ebf2618023b5",
          "name": "mail_settings.forward_bounce.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/forward_bounce?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current bounce forwarding mail settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a1aa429-e9ab-4f15-b673-4985c098d554"
            }
          ]
        }
      ]
    }
  ]
}