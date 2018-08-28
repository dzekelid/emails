{
  "info": {
    "name": "SendGrid Get Contactdb Lists",
    "_postman_id": "1b5a2f94-959d-43ea-96dc-8aa22ad7608b",
    "description": "**This endpoint allows you to retrieve all of your recipient lists. If you don't have any lists, an empty array will be returned.**\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "ece0d280-4534-4ff8-a519-4a241c0383c5",
          "name": "contactdb.lists.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/lists?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all of your recipient lists"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0417a16-d362-412d-b067-d7ffdfc279fa"
            }
          ]
        }
      ]
    }
  ]
}