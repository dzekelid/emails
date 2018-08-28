{
  "info": {
    "name": "SendGrid Get Contactdb Recipients Recipient",
    "_postman_id": "7ba8ef70-baa9-4b5f-9e71-7feca4db8d88",
    "description": "**This endpoint allows you to retrieve a single recipient by ID from your contact database.**\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "d124d872-ec50-4d58-ae49-b8eca834a80e",
          "name": "contactdb.recipients.recipient_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "contactdb/recipients/:recipient_id"
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
                  "id": "recipient_id",
                  "value": "recipient_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a single recipient by ID from your contact database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9675241b-5b53-4481-b432-9349c4bfd238"
            }
          ]
        }
      ]
    }
  ]
}