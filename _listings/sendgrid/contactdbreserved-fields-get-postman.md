{
  "info": {
    "name": "SendGrid Get Contactdb Reserved Fields",
    "_postman_id": "69064639-97e6-4941-97bd-3181c3f9981d",
    "description": "**This endpoint allows you to list all fields that are reserved and can't be used for custom field names.**\n\nThe contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "89e8e722-4569-425e-b1bf-384969b491b0",
          "name": "contactdb.reserved_fields.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/reserved_fields?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to list all fields that are reserved and can't be used for custom field names"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f999b66d-bbc6-422b-8068-1632f8e76585"
            }
          ]
        }
      ]
    }
  ]
}