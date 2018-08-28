{
  "info": {
    "name": "Dyn Retrieve Suppression Email Addresses",
    "_postman_id": "5fc98aed-87eb-4781-8022-fe7714968f2f",
    "description": "Retrieving a list of Email addresses on the suppression list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "32cf23a9-1681-4bae-9ca9-ca72cc1c39a4",
          "name": "getAccounts",
          "request": {
            "url": "http://example.com/api/accounts?apikey=%7B%7D&startindex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a list of up to 25 Email Sub-Accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05b581ab-c2b3-486e-a7ef-7aedd94b6229"
            }
          ]
        },
        {
          "id": "5192c6e3-ee91-47c6-bcca-fde55c75adbd",
          "name": "getRecipientsStatus",
          "request": {
            "url": "http://example.com/api/recipients/status?apikey=%7B%7D&emailaddress=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Recipient(s) Status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "803121fb-e503-4d59-a06a-d0f60c31673f"
            }
          ]
        },
        {
          "id": "c9bd01bf-478b-4711-980e-ee84fa0e7aac",
          "name": "getReportsBounces",
          "request": {
            "url": "http://example.com/api/reports/bounces?apikey=%7B%7D&bounce_code - Indicates the code associated with the bounced Email.=%7B%7D&bounce_code_id - The numeric code determined by the bounce processor.=%7B%7D&bounce_rule - Indicates the rule that caused this email to bounce.=%7B%7D&bounce_type=%7B%7D&bounce_type_id - Indicates whether the bounce type is a hard or soft bounce.nValid Values:n1 - Hard Bouncen2 - Soft Bounce=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&noheaders=%7B%7D&sender=%7B%7D&sender_id=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving the Email SPAM Complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "827bf90f-869b-424f-a0cb-5a38d7227e5a"
            }
          ]
        },
        {
          "id": "dde28e1f-8587-41d1-acba-909b21c62ff4",
          "name": "getReportsBouncesCount",
          "request": {
            "url": "http://example.com/api/reports/bounces/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email bounces using the API requires specific syntax for the REST API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dcedbd4-d095-4ee2-95a0-b479f3491cde"
            }
          ]
        },
        {
          "id": "15986b54-e701-4bd3-8c8d-fb279e976bd8",
          "name": "getReportsClicksCount",
          "request": {
            "url": "http://example.com/api/reports/clicks/count?apikey=%7B%7D&domainu00a0=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total of Email links clicked"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf31d781-6ab7-41e4-9d1d-2e17faad1d5c"
            }
          ]
        },
        {
          "id": "ba68c4ee-dd59-4701-be57-a49e958dd6d7",
          "name": "getReportsClicksCountUnique",
          "request": {
            "url": "http://example.com/api/reports/clicks/count/unique?apikey=%7B%7D&domainu00a0=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total of Email links clicked"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35e68886-db6f-4456-b0be-575f93007241"
            }
          ]
        },
        {
          "id": "8baad38f-1a55-4713-807a-2b3c47da5b6d",
          "name": "getReportsComplaints",
          "request": {
            "url": "http://example.com/api/reports/complaints?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Email SPAM Complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76c357c2-514b-40b3-8b1d-3872c181e10d"
            }
          ]
        },
        {
          "id": "5a79dec4-2572-457b-ad5e-b13a8d2da51a",
          "name": "getReportsComplaintsCount",
          "request": {
            "url": "http://example.com/api/reports/complaints/count?apikey=%7B%7D&endtime=%7B%7D&starttime=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5cf9007-61d4-4668-8685-3cf1f0ea499d"
            }
          ]
        },
        {
          "id": "d7274fb3-6d6d-4931-9d80-d47897502ccd",
          "name": "getReportsDelivered",
          "request": {
            "url": "http://example.com/api/reports/delivered?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Emails Delivered"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0857dd64-6236-47e4-a98b-6a3c9d83c5fd"
            }
          ]
        },
        {
          "id": "a18e7fc4-baaa-48bc-b4e0-46570d50ff22",
          "name": "getReportsDeliveredCount",
          "request": {
            "url": "http://example.com/api/reports/delivered/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Count of Emails Delivered"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4736fed4-b18e-4c8a-b7d0-23ab57645714"
            }
          ]
        },
        {
          "id": "783f7642-7018-4903-9028-6f924365a938",
          "name": "getReportsIssues",
          "request": {
            "url": "http://example.com/api/reports/issues?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&sender_id=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Email Issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d4d13d4-7302-4591-b8a8-415c0fb1287d"
            }
          ]
        },
        {
          "id": "f701952c-46c9-4488-8a59-95f693276939",
          "name": "getReportsIssuesCount",
          "request": {
            "url": "http://example.com/api/reports/issues/count?apikey=%7B%7D&endtime=%7B%7D&starttime=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9e7478d-9c79-452f-9478-02859e14a34d"
            }
          ]
        },
        {
          "id": "54096026-867b-4afd-a1f2-9eb393cb2d82",
          "name": "getReportsOpensCountUnique",
          "request": {
            "url": "http://example.com/api/reports/opens/count/unique?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns total number of unique opens for the specified account for the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2364000-4e31-4c05-b50b-4b7084a33f17"
            }
          ]
        },
        {
          "id": "277de1eb-0db4-415c-8052-743a6b75ebc1",
          "name": "getReportsSent",
          "request": {
            "url": "http://example.com/api/reports/sent?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Emails Sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "105a0d0d-77e2-4731-afd9-a610d79a81a2"
            }
          ]
        },
        {
          "id": "b5138c81-5be1-422c-a51f-4dd0b699b9d6",
          "name": "getReportsSentCount",
          "request": {
            "url": "http://example.com/api/reports/sent/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Count of Emails Sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30e12f3b-9dbe-444d-9a24-9cfd3fa98c8b"
            }
          ]
        },
        {
          "id": "cf637f36-3ff5-4c39-a1e9-9e32b80f25e2",
          "name": "getSuppressions",
          "request": {
            "url": "http://example.com/api/suppressions?apikey=%7B%7D&startdate=%7B%7D&startindex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a list of Email addresses on the suppression list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f0b5113-1d4a-46e7-a303-6a5a0641440c"
            }
          ]
        }
      ]
    },
    {
      "name": "Updating.Email",
      "item": [
        {
          "id": "7ea22298-6e59-435a-bfa3-faee873e79b7",
          "name": "putAccounts",
          "request": {
            "url": "http://example.com/api/accounts?address=%7B%7D&apikey=%7B%7D&bounceurl=%7B%7D&city=%7B%7D&companyname=%7B%7D&country=%7B%7D&generatenewapikey=%7B%7D&password=%7B%7D&phone=%7B%7D&spamurl=%7B%7D&state=%7B%7D&timezone=%7B%7D&tracklinks=%7B%7D&trackopens=%7B%7D&trackunsubscribes=%7B%7D&unsubscribeurl=%7B%7D&username=%7B%7D&zipcode=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updating an Email Sub-Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eaf263f6-72a1-4d47-bc86-79ddc20bf435"
            }
          ]
        }
      ]
    },
    {
      "name": "Create.Email",
      "item": [
        {
          "id": "9403d9b2-e325-4146-a594-1514bf9251a5",
          "name": "postAccounts",
          "request": {
            "url": "http://example.com/api/accounts?address=%7B%7D&apikey=%7B%7D&bounceurl=%7B%7D&city=%7B%7D&companyname=%7B%7D&country=%7B%7D&generatenewapikey=%7B%7D&password=%7B%7D&phone=%7B%7D&spamurl=%7B%7D&state=%7B%7D&timezone=%7B%7D&tracklinks=%7B%7D&trackopens=%7B%7D&trackunsubscribes=%7B%7D&username=%7B%7D&zipcode=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creating an Email Sub-Account using the API requires specific syntax for the REST API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06726746-b4b1-42c8-b0e1-06385b058dc6"
            }
          ]
        }
      ]
    },
    {
      "name": "Deleting.Email",
      "item": [
        {
          "id": "b6a4b618-5aea-4089-a2f1-8f25ded4f841",
          "name": "postAccountsDelete",
          "request": {
            "url": "http://example.com/api/accounts/delete?apikey=%7B%7D&username=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Deleting an Email Sub-Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8d46402-5431-48ea-b068-e9d2aed75624"
            }
          ]
        }
      ]
    },
    {
      "name": ".Email",
      "item": [
        {
          "id": "92d12861-886a-46cc-ae7b-338ecebc2ff4",
          "name": "getOpensCount",
          "request": {
            "url": "http://example.com/api/opens/count?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns total number of opens for the specified account for the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a16d471-ed37-4afa-9f50-e0bf23f17dba"
            }
          ]
        }
      ]
    },
    {
      "name": "Activate",
      "item": [
        {
          "id": "2c4ad653-4d71-49f8-9a85-e0f7e49014ff",
          "name": "postRecipientsActivate",
          "request": {
            "url": "http://example.com/api/recipients/activate?apikey=%7B%7D&emailaddress=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Activating a specified Recipientu2019s status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c93c4ee-b81b-48a6-a85a-ca2fa01df411"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "1e389232-0be7-47cf-9e83-d1a2f01546cb",
          "name": "getReportsClicks",
          "request": {
            "url": "http://example.com/api/reports/clicks?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of links clicked for the specified account during the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62c78469-64e0-479f-925c-b372f67afacb"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique",
      "item": [
        {
          "id": "e74d3fba-5291-44be-be76-f9172cccb351",
          "name": "getReportsClicksUnique",
          "request": {
            "url": "http://example.com/api/reports/clicks/unique?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of unique links clicked for the specified account during the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "267156ec-9d80-4d7d-b679-0d078082975c"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "dde80f39-7732-4456-9242-0db14423ecc4",
          "name": "postSend",
          "request": {
            "url": "http://example.com/api/send?apikey=%7B%7D&bcc=%7B%7D&bodyhtml=%7B%7D&bodytext=%7B%7D&cc=%7B%7D&comments=%7B%7D&from=%7B%7D&importance=%7B%7D&inreplyto=%7B%7D&keywords=%7B%7D&messageid=%7B%7D&priority=%7B%7D&references=%7B%7D&replyby=%7B%7D&replyto=%7B%7D&resent-date=%7B%7D&resent-from=%7B%7D&resent-messageid=%7B%7D&resent-replyto=%7B%7D&resent-sender=%7B%7D&sender=%7B%7D&sensitivity=%7B%7D&subject=%7B%7D&to=%7B%7D&xheaders=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sending Email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27a3f94e-3b4b-4dec-a62a-318aed05f276"
            }
          ]
        }
      ]
    }
  ]
}