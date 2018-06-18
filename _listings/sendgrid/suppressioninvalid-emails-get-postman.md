{
  "info": {
    "name": "SendGrid Get Suppression Inval Emails",
    "_postman_id": "849fdd6c-e8a9-4e43-91c5-e8e072104c88",
    "description": "**This endpoint allows you to retrieve a list of all invalid email addresses.**\n\nAn invalid email occurs when you attempt to send email to an address that is formatted in a manner that does not meet internet email format standards or the email does not exist at the recipient’s mail server.\n\nExamples include addresses without the “@” sign or addresses that include certain special characters and/or spaces. This response can come from our own server or the recipient mail server.\n\nFor more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "3dfe2283-570f-4efe-9b48-0c8fee179c3a",
          "name": "suppression.invalid_emails.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/suppression/invalid_emails?end_time=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&start_time=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all invalid email addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "739994b2-db6d-4b95-827b-8a628eaf4d7d"
            }
          ]
        }
      ]
    }
  ]
}