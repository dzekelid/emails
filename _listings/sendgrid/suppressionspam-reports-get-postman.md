{
  "info": {
    "name": "SendGrid Get Suppression Spam Reports",
    "_postman_id": "53559250-2d08-4b8c-bc4b-a2512d7eb5d7",
    "description": "**This endpoint allows you to retrieve all spam reports.**\n\n[Spam reports](https://sendgrid.com/docs/Glossary/spam_reports.html) happen when a recipient indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html) and then their email provider reports this to SendGrid.\n\nFor more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "0125524a-be0f-4627-bdb7-1bcf087ab286",
          "name": "suppression.spam_reports.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/suppression/spam_reports?end_time=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&start_time=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all spam reports"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb41ba1a-ca04-4b09-a7a7-f8acf6b487c9"
            }
          ]
        }
      ]
    }
  ]
}