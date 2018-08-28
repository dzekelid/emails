{
  "info": {
    "name": "AWS Simple Email Service API List Verified Email Addresses",
    "_postman_id": "33c415ae-63e3-432b-86e2-416678c6ef45",
    "description": "Returns a list containing all of the email addresses that have been verified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "ffedafe8-fb5d-4d59-8e53-6b738f2e08be",
          "name": "deleteVerifiedEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVerifiedEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified email address from the list of verified addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9837a41a-21b8-445c-8eca-2b7104e6b21f"
            }
          ]
        },
        {
          "id": "26f497a9-0d9d-4366-bb4d-958411efde0e",
          "name": "listVerifiedEmailAddresses",
          "request": {
            "url": "http://example.com/api/?Action=ListVerifiedEmailAddresses?VerifiedEmailAddresses.member.N=VerifiedEmailAddresses.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the email addresses that have been verified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f4fe5f1-25f0-4e18-ace4-5696e94051a4"
            }
          ]
        }
      ]
    }
  ]
}