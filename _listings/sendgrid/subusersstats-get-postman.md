{
  "info": {
    "name": "SendGrid Get Subusers Stats",
    "_postman_id": "2067e328-1eae-4890-b465-032a51679c02",
    "description": "**This endpoint allows you to retrieve the email statistics for the given subusers.**\n\nYou may retrieve statistics for up to 10 different subusers by including an additional _subusers_ parameter for each additional subuser.\n\nWhile you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.\n\nFor more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "592660e9-f292-420e-8923-20f558206be4",
          "name": "subusers.stats.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/subusers/stats?aggregated_by=%7B%7D&end_date=%7B%7D&limit=%7B%7D&offset=%7B%7D&start_date=%7B%7D&subusers=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve the email statistics for the given subusers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76f1a263-8418-41dc-8bbb-17fc6525022f"
            }
          ]
        }
      ]
    }
  ]
}