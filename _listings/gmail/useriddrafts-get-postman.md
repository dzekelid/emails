{
  "info": {
    "name": "Gmail Get Drafts",
    "_postman_id": "b89c51ae-6527-43fe-8331-9053ae563b62",
    "description": "Lists the drafts in the user's mailbox.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Email",
      "item": [
        {
          "id": "ab2ee5f4-9463-4c8e-8ee5-9e46fe56203b",
          "name": "gmail.users.drafts.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "gmail",
                "v1",
                "users",
                ":userId/drafts"
              ],
              "query": [
                {
                  "key": "includeSpamTrash",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "q",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "userId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the drafts in the user's mailbox."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13b5d2d2-f484-4de6-b553-18de82a2c040"
            }
          ]
        }
      ]
    }
  ]
}