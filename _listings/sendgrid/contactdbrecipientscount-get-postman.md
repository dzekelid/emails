{
  "info": {
    "name": "SendGrid Get Contactdb Recipients Count",
    "_postman_id": "1bab79dc-bd77-483a-aa8b-b9c048f6c73c",
    "description": "**This endpoint allows you to retrieve the total number of Marketing Campaigns recipients.**\n\nThe contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "6f119666-fbf1-4971-85b8-13ecad5b13e3",
          "name": "contactdb.recipients.count.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/recipients/count?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve the total number of Marketing Campaigns recipients"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66bd0059-67b8-4f0c-b53f-cd183c9e7c59"
            }
          ]
        }
      ]
    }
  ]
}