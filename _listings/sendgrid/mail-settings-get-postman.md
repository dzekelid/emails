{
  "info": {
    "name": "SendGrid Get Mail Settings",
    "_postman_id": "c927331a-ea04-4edf-9424-128061a6d517",
    "description": "**This endpoint allows you to retrieve a list of all mail settings.**\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "1630a423-23f2-4d55-95f2-7c45086fec38",
          "name": "GET_mail_settings",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings?limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all mail settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "308de63b-57fe-4afa-a01b-7eb9eba20798"
            }
          ]
        }
      ]
    }
  ]
}