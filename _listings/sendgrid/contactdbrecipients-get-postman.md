{
  "info": {
    "name": "SendGrid Get Contactdb Recipients",
    "_postman_id": "7487f8dc-bcad-4fa3-a5cf-1cdb8141b5eb",
    "description": "**This endpoint allows you to retrieve all of your Marketing Campaigns recipients.**\n\nBatch deletion of a page makes it possible to receive an empty page of recipients before reaching the end of\nthe list of recipients. To avoid this issue; iterate over pages until a 404 is retrieved.\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "27869b15-5aac-40bb-a7b9-17a621a0f120",
          "name": "contactdb.recipients.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/recipients?No Name=%7B%7D&page=%7B%7D&page_size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all of your Marketing Campaigns recipients"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ed2a28f-a738-4a0a-98b7-aa112a7924f3"
            }
          ]
        }
      ]
    }
  ]
}