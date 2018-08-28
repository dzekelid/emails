{
  "info": {
    "name": "SendGrid Get Contactdb Lists List  Recipients",
    "_postman_id": "95c15e43-c1e8-4406-870d-e218ad665f17",
    "description": "**This endpoint allows you to retrieve all recipients on the list with the given ID.** \n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "5f1b353a-5b7a-4825-b459-0b8ddc773b9b",
          "name": "contactdb.lists.list_id.recipients.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "contactdb/lists/:list_id/recipients"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "list_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all recipients on the list with the given ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a7c54a9-d2df-4c48-ac27-c0960daf05c6"
            }
          ]
        }
      ]
    }
  ]
}