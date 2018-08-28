{
  "info": {
    "name": "SendGrid Delete Scopes Requests Request",
    "_postman_id": "7a5c2a05-82c8-40f0-beab-93a325edea39",
    "description": "This endpoint allows you to deny an attempt to access your account.\n\n**Note:** Only teammate admins may delete a teammate's access request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "d145bcc1-1f16-4f4d-9282-4ac337bfc391",
          "name": "scopes.requests.request_id.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "scopes/requests/:request_id"
              ],
              "variable": [
                {
                  "id": "request_id",
                  "value": "request_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint allows you to deny an attempt to access your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4399455e-1fd4-45fc-bc70-fbdb095afd28"
            }
          ]
        }
      ]
    }
  ]
}