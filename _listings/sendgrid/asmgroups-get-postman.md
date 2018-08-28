{
  "info": {
    "name": "SendGrid Get Asm Groups",
    "_postman_id": "2159d41b-da00-4d07-912c-c93d55a413ca",
    "description": "**This endpoint allows you to retrieve information about multiple suppression groups.**\n\nThis endpoint will return information for each group ID that you include in your request. To add a group ID to your request, simply append `&id=` followed by the group ID.\n\nSuppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).\n\nSuppression groups, or [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html), allow you to label a category of content that you regularly send. This gives your recipients the ability to opt out of a specific set of your email. For example, you might define a group for your transactional email, and one for your marketing email so that your users can continue recieving your transactional email witout having to receive your marketing content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "3b15b6d9-56a7-424e-b138-e4119edbdf6e",
          "name": "asm.groups.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/asm/groups?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve information about multiple suppression groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c55588d-265a-4f82-abe8-ff7f81349a33"
            }
          ]
        }
      ]
    }
  ]
}