{
  "info": {
    "name": "SendGrid Get Api Keys Api Key",
    "_postman_id": "83c33574-4b1a-418e-b122-0db1819b2978",
    "description": "**This endpoint allows you to retrieve a single api key.**\n\nIf the API Key ID does not exist an HTTP 404 will be returned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "71a90ae1-89b7-4af2-a013-2ee5b950ae04",
          "name": "api_keys.api_key_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "api_keys/:api_key_id"
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
                  "id": "api_key_id",
                  "value": "api_key_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a single api key"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d71b7bcd-cc41-486f-9cfe-bfd29ac655f5"
            }
          ]
        }
      ]
    }
  ]
}