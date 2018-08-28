{
  "info": {
    "name": "SendGrid Get Contactdb Custom Fields Custom Field",
    "_postman_id": "5cbd05f0-a19b-4a37-99e5-dc0d216bb2b6",
    "description": "**This endpoint allows you to retrieve a custom field by ID.**\n\nThe contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "6033eb5f-aa6d-4b4a-ad5a-8ff5d7b6824f",
          "name": "contactdb.custom_fields.custom_field_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "contactdb/custom_fields/:custom_field_id"
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
                  "id": "custom_field_id",
                  "value": "custom_field_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a custom field by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a66eec10-32b1-4703-a0dc-31180b3b7cca"
            }
          ]
        }
      ]
    }
  ]
}