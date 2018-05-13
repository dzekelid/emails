{
  "info": {
    "name": "SendGrid Get Suppression Inval Emails Email",
    "_postman_id": "649f3ef3-83ad-4988-9eaa-44d5a35b3a35",
    "description": "**This endpoint allows you to retrieve a specific invalid email addresses.**\n\nAn invalid email occurs when you attempt to send email to an address that is formatted in a manner that does not meet internet email format standards or the email does not exist at the recipient’s mail server.\n\nExamples include addresses without the “@” sign or addresses that include certain special characters and/or spaces. This response can come from our own server or the recipient mail server.\n\nFor more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "ccb1ac93-f31b-484f-9b34-248f38198a0e",
          "name": "suppression.invalid_emails.email.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "suppression/invalid_emails/:email"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "email",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a specific invalid email addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36cd79fb-9b0d-4001-81f4-d64627153097"
            }
          ]
        }
      ]
    }
  ]
}