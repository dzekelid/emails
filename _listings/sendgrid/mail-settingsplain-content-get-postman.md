{
  "info": {
    "name": "SendGrid Get Mail Settings Plain Content",
    "_postman_id": "9afd87b2-9067-4ea7-928a-cb7d0e431de7",
    "description": "**This endpoint allows you to retrieve your current Plain Content mail settings.**\n\nThe plain content setting will automatically convert any plain text emails that you send to HTML before sending.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "69f49f7e-85a7-46cb-9e8a-407ef00daa63",
          "name": "mail_settings.plain_content.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/plain_content?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current Plain Content mail settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cec6c1d8-b941-4b36-9347-4e26b973aecb"
            }
          ]
        }
      ]
    }
  ]
}