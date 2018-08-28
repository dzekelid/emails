{
  "info": {
    "name": "SendGrid Get Mail Settings Footer",
    "_postman_id": "3d4f9d97-a837-4ebb-8df3-5b3653695b04",
    "description": "**This endpoint allows you to retrieve your current Footer mail settings.**\n\nThe footer setting will insert a custom footer at the bottom of the text and HTML bodies. Use the embedded HTML editor and plain text entry fields to create the content of the footers to be inserted into your emails.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "2a5bb427-effd-4bf7-ac28-25ee70a304b2",
          "name": "mail_settings.footer.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/footer?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current Footer mail settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71cdaa3f-d0d3-4039-aa9b-b3523f5107f2"
            }
          ]
        }
      ]
    }
  ]
}