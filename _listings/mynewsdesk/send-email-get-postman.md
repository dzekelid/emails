{
  "info": {
    "name": "My News Desk Pressroom List Send Email",
    "_postman_id": "5f11e937-6d51-4c38-9449-9d3ddde87187",
    "description": "Send Email",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Send",
      "item": [
        {
          "id": "f21d68ca-e6b6-4e01-aa42-e700a1093a43",
          "name": "getSendEmail",
          "request": {
            "url": "http://www.mynewsdesk.com/services/pressroom/send_email/?from=%7B%7D&item_id=%7B%7D&message=%7B%7D&to_email=%7B%7D&type_of_media=%7B%7D&unique key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Send Email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcf977b6-6808-49e9-ad42-a861c60b3bd5"
            }
          ]
        }
      ]
    }
  ]
}