{
  "info": {
    "name": "SendGrid Get Mail Settings Forward Spam",
    "_postman_id": "54320a42-ad04-4ef0-bc65-d8de842a4e7c",
    "description": "**This endpoint allows you to retrieve your current Forward Spam mail settings.**\n\nEnabling the forward spam setting allows you to specify an email address to which spam reports will be forwarded.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "5fa8e043-449b-44d3-ae87-14850680f870",
          "name": "mail_settings.forward_spam.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/forward_spam?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current Forward Spam mail settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74b2af69-02f7-44e9-8c58-081a4bd71891"
            }
          ]
        }
      ]
    }
  ]
}