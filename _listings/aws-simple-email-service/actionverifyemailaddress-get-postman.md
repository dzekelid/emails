{
  "info": {
    "name": "AWS Simple Email Service API Verify Email Address",
    "_postman_id": "d57350ce-b89e-48c7-8e56-8f9459786ffc",
    "description": "Verifies an email address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "088442d6-82aa-46ff-b564-710795ce5881",
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
              "id": "4032b389-89cb-4f3a-aad3-4741219a9138"
            }
          ]
        },
        {
          "id": "ec49b9f2-c257-4e86-a328-a3ed96614fda",
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
              "id": "2f33d563-15ed-4f05-b6f0-5856fe21df30"
            }
          ]
        }
      ]
    },
    {
      "name": "Email Addresses",
      "item": [
        {
          "id": "eddfb1d0-186e-48bb-b54b-c5e74c85d905",
          "name": "verifyEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=VerifyEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies an email address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03691ff6-dd4a-4d5a-8b32-7ce52b5c4d04"
            }
          ]
        }
      ]
    }
  ]
}