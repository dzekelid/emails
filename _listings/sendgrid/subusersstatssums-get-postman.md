{
  "info": {
    "name": "SendGrid Get Subusers Stats Sums",
    "_postman_id": "a892a835-a89e-41ab-8bcf-4dfd0253d356",
    "description": "**This endpoint allows you to retrieve the total sums of each email statistic metric for all subusers over the given date range.**\n\n\nWhile you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.\n\nFor more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "d8ddfed5-2464-46b7-905b-e539915d1d92",
          "name": "subusers.stats.sums.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/subusers/stats/sums?aggregated_by=%7B%7D&end_date=%7B%7D&limit=%7B%7D&offset=%7B%7D&sort_by_direction=%7B%7D&sort_by_metric=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve the total sums of each email statistic metric for all subusers over the given date range"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd3d7ff3-8481-4624-a55e-68d9d5706482"
            }
          ]
        }
      ]
    }
  ]
}