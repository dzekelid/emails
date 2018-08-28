{
  "info": {
    "name": "SendGrid Delete Senders Sender",
    "_postman_id": "97ee8ce5-c814-45cb-85ad-d9ccc477c1c2",
    "description": "**This endoint allows you to delete one of your sender identities.**\n\nSender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "134847d2-d308-43ca-963d-29367c77072c",
          "name": "senders.sender_id.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "**This endoint allows you to delete one of your sender identities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0a86b62-77be-4df9-adef-0d295e369452"
            }
          ]
        }
      ]
    }
  ]
}