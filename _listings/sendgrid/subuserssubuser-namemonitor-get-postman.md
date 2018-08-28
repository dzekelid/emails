{
  "info": {
    "name": "SendGrid Get Subusers Subuser Name Monitor",
    "_postman_id": "f66d9135-59a3-41e9-98f8-782fadb6f196",
    "description": "Subuser monitor settings allow you to receive a sample of an outgoing message by a specific customer at a specific frequency of emails.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "2b8e7596-32cc-4bf6-81a3-e683dd3cc1c4",
          "name": "subusers.subuser_name.monitor.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "subusers/:subuser_name/monitor"
              ],
              "variable": [
                {
                  "id": "subuser_name",
                  "value": "subuser_name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Subuser monitor settings allow you to receive a sample of an outgoing message by a specific customer at a specific frequency of emails"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "616050b4-8c1b-4a7b-bd83-9074ad7464d4"
            }
          ]
        }
      ]
    }
  ]
}