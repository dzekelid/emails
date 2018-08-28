{
  "info": {
    "name": "SendGrid Get Contactdb Custom Fields",
    "_postman_id": "ef3c4040-d0a1-47d1-9d45-2b03b20e735a",
    "description": "**This endpoint allows you to retrieve all custom fields.** \n\nThe contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "ae920ed3-037f-4204-a1e8-2c023c89417f",
          "name": "contactdb.custom_fields.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/custom_fields?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all custom fields"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81fbac1d-aee1-43f6-a2f2-0047dcecdac5"
            }
          ]
        }
      ]
    }
  ]
}