{
  "info": {
    "name": "SendGrid Get Asm Groups Group  Suppressions",
    "_postman_id": "3fc03ce6-5ca2-4dc5-a2dc-34e5a2d30f7a",
    "description": "**This endpoint allows you to retrieve all suppressed email addresses belonging to the given group.**\n\nSuppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "3a51f4a2-7843-4c36-b7fe-96221355caf2",
          "name": "asm.groups.group_id.suppressions.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "asm/groups/:group_id/suppressions"
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
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all suppressed email addresses belonging to the given group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4590c39-0de0-4d49-bf1a-82816d973843"
            }
          ]
        }
      ]
    }
  ]
}