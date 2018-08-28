{
  "info": {
    "name": "SendGrid Delete User Webhooks Parse Settings Hostname",
    "_postman_id": "d8968bcd-8af3-4a3c-ab17-a9d4f25d2f44",
    "description": "**This endpoint allows you to delete a specific inbound parse setting.**\n\nThe inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "70b74266-5b8b-4e03-9aaa-8630aa3a8903",
          "name": "user.webhooks.parse.settings.hostname.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to delete a specific inbound parse setting"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "453ed7bc-7710-43ba-821b-f2e5f763e650"
            }
          ]
        }
      ]
    }
  ]
}