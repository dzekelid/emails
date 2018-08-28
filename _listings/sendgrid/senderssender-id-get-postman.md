{
  "info": {
    "name": "SendGrid Get Senders Sender",
    "_postman_id": "f67dfb1b-40e1-4b99-8171-1c0215990f07",
    "description": "**This endpoint allows you to retrieve a specific sender identity.**\n\nSender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "5f0477d9-a7fe-4f4e-878d-97d8c76646b9",
          "name": "senders.sender_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "senders/:sender_id"
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
                  "id": "sender_id",
                  "value": "sender_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a specific sender identity"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9a2139c-f83d-4084-985f-533c45acaddd"
            }
          ]
        }
      ]
    }
  ]
}