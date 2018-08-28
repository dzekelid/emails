{
  "info": {
    "name": "SendGrid Get Contactdb Recipients Search",
    "_postman_id": "68613b5e-87d4-4db3-8e0a-95bde3b8b268",
    "description": "**This endpoint allows you to perform a search on all of your Marketing Campaigns recipients.**\n\nfield_name:\n\n* is a variable that is substituted for your actual custom field name from your recipient.\n* Text fields must be url-encoded. Date fields are searchable only by unix timestamp (e.g. 2/2/2015 becomes 1422835200)\n* If field_name is a 'reserved' date field, such as created_at or updated_at, the system will internally convert\nyour epoch time to a date range encompassing the entire day. For example, an epoch time of 1422835600 converts to\nMon, 02 Feb 2015 00:06:40 GMT, but internally the system will search from Mon, 02 Feb 2015 00:00:00 GMT through\nMon, 02 Feb 2015 23:59:59 GMT.\n\nThe contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "87b3f043-c534-4e7e-994b-2b79bcccc646",
          "name": "contactdb.recipients.search.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/contactdb/recipients/search?No Name=%7B%7D&{field_name}=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to perform a search on all of your Marketing Campaigns recipients"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb09caa1-38fe-48ea-87ac-e460f06991f8"
            }
          ]
        }
      ]
    }
  ]
}