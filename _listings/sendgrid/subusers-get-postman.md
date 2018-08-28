{
  "info": {
    "name": "SendGrid Get Subusers",
    "_postman_id": "f4fbca1f-dfc2-4df5-ad69-e94cb451ae38",
    "description": "This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.\n\nFor more information about Subusers:\n\n* [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)\n* [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "2868216b-4a5d-4547-8252-5a8c8d023787",
          "name": "GET_subusers",
          "request": {
            "url": "http://api.sendgrid.com/v3/subusers?limit=%7B%7D&offset=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint allows you to retrieve a list of all of your subusers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56f15efd-8af6-470f-9760-2315432c0d35"
            }
          ]
        }
      ]
    }
  ]
}