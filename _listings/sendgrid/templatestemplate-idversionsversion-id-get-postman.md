{
  "info": {
    "name": "SendGrid Get Templates Template  Versions Version",
    "_postman_id": "bda913bc-9894-48a2-b2d1-a5d91523f976",
    "description": "**This endpoint allows you to retrieve a specific version of a template.**\n\nEach transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.\n\nFor more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).\n\n## URI Parameters\n| URI Parameter | Type | Description |\n|---|---|---|\n| template_id | string | The ID of the original template |\n| version_id | string |  The ID of the template version |",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "54d72da5-3ebc-4efd-9e89-efe757a9b537",
          "name": "templates.template_id.versions.version_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "templates/:template_id/versions/:version_id"
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
                  "id": "template_id",
                  "value": "template_id",
                  "type": "string"
                },
                {
                  "id": "version_id",
                  "value": "version_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a specific version of a template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08156729-9ba9-4256-8669-f9cfa3e55ed5"
            }
          ]
        }
      ]
    }
  ]
}