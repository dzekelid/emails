{
  "info": {
    "name": "SendGrid Get Contactdb Segments Segment  Recipients",
    "_postman_id": "efcc1af9-f986-48e8-8218-18d535997707",
    "description": "**This endpoint allows you to retrieve all of the recipients in a segment with the given ID.**\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.\n\nFor more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "5c0205a8-f71e-4d0b-8d31-161a2e9ed9d2",
          "name": "contactdb.segments.segment_id.recipients.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "contactdb/segments/:segment_id/recipients"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "segment_id",
                  "value": "segment_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all of the recipients in a segment with the given ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08931a73-8e45-42cb-8d39-f397cc42d54a"
            }
          ]
        }
      ]
    }
  ]
}