{
  "info": {
    "name": "SendGrid Get Mail Settings Bcc",
    "_postman_id": "315aeee3-e27e-460c-82e8-62c8e4bbb4dd",
    "description": "**This endpoint allows you to retrieve your current BCC mail settings.**\n\nWhen the BCC mail setting is enabled, SendGrid will automatically send a blind carbon copy (BCC) to an address for every email sent without adding that address to the header. Please note that only one email address may be entered in this field, if you wish to distribute BCCs to multiple addresses you will need to create a distribution group or use forwarding rules.\n\nMail settings allow you to tell SendGrid specific things to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "2d4d3547-354a-4966-bb09-5d99ba770cfc",
          "name": "mail_settings.bcc.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/mail_settings/bcc?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current BCC mail settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b24c68a-b635-4884-984c-e38eabc633e4"
            }
          ]
        }
      ]
    }
  ]
}