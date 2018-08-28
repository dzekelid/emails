{
  "info": {
    "name": "SendGrid Get User Webhooks Parse Settings Hostname",
    "_postman_id": "5726d1a5-7314-4a58-b2f2-1c57ee95a438",
    "description": "**This endpoint allows you to retrieve a specific inbound parse setting.**\n\nThe inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "cd4bb0dd-b7fc-4f7f-bec2-8076bfd7d3ba",
          "name": "user.webhooks.parse.settings.hostname.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "user/webhooks/parse/settings/:hostname"
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
                  "id": "hostname",
                  "value": "hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a specific inbound parse setting"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83675715-78f7-4492-9033-fa2c7682b632"
            }
          ]
        }
      ]
    }
  ]
}