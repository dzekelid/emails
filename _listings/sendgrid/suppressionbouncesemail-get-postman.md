{
  "info": {
    "name": "SendGrid Get Suppression Bounces Email",
    "_postman_id": "623a8281-dd29-445f-9c3c-349c90100aae",
    "description": "**This endpoint allows you to retrieve a specific bounce for a given email address.**\n\nA bounced email is when the message is undeliverable and then returned to the server that sent it.\n\nFor more information see: \n\n* [User Guide > Bounces](https://sendgrid.com/docs/User_Guide/Suppressions/bounces.html) for more information\n* [Glossary > Bounces](https://sendgrid.com/docs/Glossary/Bounces.html)\n* [Classroom > List Scrubbing Guide](https://sendgrid.com/docs/Classroom/Deliver/list_scrubbing.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "df650439-04ff-4b4f-9216-e886acdbd512",
          "name": "suppression.bounces.email.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "suppression/bounces/:email"
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
            "description": "**This endpoint allows you to retrieve a specific bounce for a given email address"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad4b672b-afbe-437e-8ae3-2328a37618cb"
            }
          ]
        }
      ]
    }
  ]
}