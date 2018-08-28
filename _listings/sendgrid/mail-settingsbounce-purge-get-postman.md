{
  "info": {
    "name": "SendGrid Get Mail Settings Bounce Purge",
    "_postman_id": "08b1fe19-a4c1-4426-9205-3044012b549d",
    "description": "**This endpoint allows you to retrieve your current bounce purge settings.**\n\nThis setting allows you to set a schedule for SendGrid to automatically delete contacts from your soft and hard bounce suppression lists.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "b332ef43-a6ab-4ea2-96b5-f7bf89a0f6d3",
          "name": "mail_settings.bounce_purge.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/bounce_purge?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current bounce purge settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "302ed7c1-d536-414b-97e7-58df744678c7"
            }
          ]
        }
      ]
    }
  ]
}