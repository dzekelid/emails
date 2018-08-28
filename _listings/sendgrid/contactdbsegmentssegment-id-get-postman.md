{
  "info": {
    "name": "SendGrid Get Contactdb Segments Segment",
    "_postman_id": "36e672d1-0885-4919-a2f5-84589a53eedc",
    "description": "**This endpoint allows you to retrieve a single segment with the given ID.**\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.\n\nFor more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "3929d7a2-b04f-49cc-b7ac-14cf1d6cada6",
          "name": "contactdb.segments.segment_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sendgrid.com",
              "path": [
                "v3",
                "contactdb/segments/:segment_id"
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
                  "id": "segment_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a single segment with the given ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2314ee3e-ced2-4856-b513-db63cece6193"
            }
          ]
        }
      ]
    }
  ]
}