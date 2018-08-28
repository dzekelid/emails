{
  "info": {
    "name": "SendGrid Get Contactdb Lists List",
    "_postman_id": "6d7242c3-1e27-4466-a97e-c3a8109fcf71",
    "description": "This endpoint allows you to retrieve a single recipient list.\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "4d74f132-4599-440b-a944-ea4930d68540",
          "name": "contactdb.lists.list_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "contactdb/lists/:list_id"
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
            "description": "This endpoint allows you to retrieve a single recipient list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16580d51-d138-451c-8da2-3ef3bc12a9fa"
            }
          ]
        }
      ]
    }
  ]
}