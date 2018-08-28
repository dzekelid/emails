{
  "info": {
    "name": "SendGrid Get Scopes Requests",
    "_postman_id": "a157d298-2fd4-48c5-ab65-dc9ff68be90c",
    "description": "This endpoint allows you to retrieve a list of all recent access requests.\n\n**Note:** The Response Header's 'link' parameter will include pagination info. For example:\n\nlink: ```<https://api.sendgrid.com/v3/scopes/requests?limit=10&offset=0>; rel=\"first\"; title=\"1\", <https://api.sendgrid.com/v3/scopes/requests?limit=10&offset=10>; rel=\"last\"; title=\"2\", <https://api.sendgrid.com/v3/scopes/requests?limit=10&offset=0>; rel=\"prev\"; title=\"1\"```",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "b49df1cc-c155-45e3-b113-4a527f045d18",
          "name": "scopes.requests.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/scopes/requests?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint allows you to retrieve a list of all recent access requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "665d866f-40fe-420f-a803-b59c7da30243"
            }
          ]
        }
      ]
    }
  ]
}