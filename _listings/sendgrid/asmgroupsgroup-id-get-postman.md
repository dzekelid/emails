{
  "info": {
    "name": "SendGrid Get Asm Groups Group",
    "_postman_id": "51a5bf7f-78a5-49eb-8c69-b3954974eedb",
    "description": "**This endpoint allows you to retrieve a single suppression group.**\n\nSuppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.\n\nThe **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.\n\nEach user can create up to 25 different suppression groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "9dd48d6f-3cf0-4552-a79d-ec5e6a759bfd",
          "name": "asm.groups.group_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "asm/groups/:group_id"
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
            "description": "**This endpoint allows you to retrieve a single suppression group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80278f13-1d58-4d83-8eba-6770f0167d34"
            }
          ]
        }
      ]
    }
  ]
}