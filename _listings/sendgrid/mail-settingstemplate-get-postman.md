{
  "info": {
    "name": "SendGrid Get Mail Settings Template",
    "_postman_id": "a274b9f4-e196-4995-9731-db1872e1f505",
    "description": "**This endpoint allows you to retrieve your current legacy email template settings.**\n\nThis setting refers to our original email templates. We currently support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html). \n\nThe legacy email template setting wraps an HTML template around your email content. This can be useful for sending out marketing email and/or other HTML formatted messages.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "a830adce-9fde-4ac2-82e7-82aa67d10e7d",
          "name": "mail_settings.template.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/template?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current legacy email template settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef5a1fdd-1392-460b-8dff-54e750f23354"
            }
          ]
        }
      ]
    }
  ]
}