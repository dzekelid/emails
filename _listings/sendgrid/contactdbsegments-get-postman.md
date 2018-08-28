{
  "info": {
    "name": "SendGrid Get Contactdb Segments",
    "_postman_id": "c97ba462-6d46-404a-a8dd-a1bba5a6e00d",
    "description": "**This endpoint allows you to retrieve all of your segments.**\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.\n\nFor more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "7e0bc41c-ba21-446b-9567-9b245d10ac29",
          "name": "contactdb.segments.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/segments?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all of your segments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bc9eeef-a3d1-40db-adb8-d456188a28a7"
            }
          ]
        }
      ]
    }
  ]
}