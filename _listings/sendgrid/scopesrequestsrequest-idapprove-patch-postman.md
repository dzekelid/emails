{
  "info": {
    "name": "SendGrid Patch Scopes Requests Request  Approve",
    "_postman_id": "a53bb5c5-cd89-4940-9648-ace5a7f96149",
    "description": "This endpoint allows you to approve an access attempt.\n\n**Note:** Only teammate admins may approve another teammate???s access request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "38914a48-3e1d-44bc-ac81-d3a81b8ad33c",
          "name": "scopes.requests.request_id.approve.patch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "scopes/requests/:request_id/approve"
              ],
              "variable": [
                {
                  "id": "request_id",
                  "value": "request_id",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint allows you to approve an access attempt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04072ade-b025-4b6f-b28f-91cfbea264d2"
            }
          ]
        }
      ]
    }
  ]
}