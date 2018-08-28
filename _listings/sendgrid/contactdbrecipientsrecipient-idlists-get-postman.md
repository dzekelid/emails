{
  "info": {
    "name": "SendGrid Get Contactdb Recipients Recipient  Lists",
    "_postman_id": "af976ecb-4c3e-40c0-abc7-ed0b78b0341f",
    "description": "**This endpoint allows you to retrieve the lists that a given recipient belongs to.**\n\nEach recipient can be on many lists. This endpoint gives you all of the lists that any one recipient has been added to.\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "811cb1f8-4d93-4a7e-a1d6-760f2def6c33",
          "name": "contactdb.recipients.recipient_id.lists.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "contactdb/recipients/:recipient_id/lists"
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
            "description": "**This endpoint allows you to retrieve the lists that a given recipient belongs to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "448aabc9-ceee-4dea-ae59-0f49f5b46c4e"
            }
          ]
        }
      ]
    }
  ]
}