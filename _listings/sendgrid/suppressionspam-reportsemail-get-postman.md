{
  "info": {
    "name": "SendGrid Get Suppression Spam Reports Email",
    "_postman_id": "4621e5ff-d973-4a95-aba8-89f3976622ea",
    "description": "**This endpoint allows you to retrieve a specific spam report.**\n\n[Spam reports](https://sendgrid.com/docs/Glossary/spam_reports.html) happen when a recipient indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html) and then their email provider reports this to SendGrid.\n\nFor more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "8e125980-7992-4f39-bfaa-4d73a4a28beb",
          "name": "suppression.spam_reports.email.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "suppression/spam_reports/:email"
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
            "description": "**This endpoint allows you to retrieve a specific spam report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc6931a7-a417-41d9-8958-19199f396eee"
            }
          ]
        }
      ]
    }
  ]
}