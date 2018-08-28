{
  "info": {
    "name": "SendGrid Get User Settings Enforced Tls",
    "_postman_id": "25c6e3d1-2d2b-445e-bd8c-fb62cccee849",
    "description": "**This endpoint allows you to retrieve your current Enforced TLS settings.**\n\nThe Enforced TLS settings specify whether or not the recipient is required to support TLS or have a valid certificate. See the [SMTP Ports User Guide](https://sendgrid.com/docs/Classroom/Basics/Email_Infrastructure/smtp_ports.html) for more information on opportunistic TLS.\n\n**Note:** If either setting is enabled and the recipient does not support TLS or have a valid certificate, we drop the message and send a block event with ???TLS required but not supported??? as the description.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "4d15b180-63dc-42ee-bffd-d5b8df1f4d83",
          "name": "user.settings.enforced_tls.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/user/settings/enforced_tls?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your current Enforced TLS settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af79b5b0-7fd0-4382-96ae-effdd2666649"
            }
          ]
        }
      ]
    }
  ]
}