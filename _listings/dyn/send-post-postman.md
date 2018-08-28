{
  "info": {
    "name": "Dyn Send Email",
    "_postman_id": "48a3bddf-1e28-4ef7-afe9-2d5db959f35d",
    "description": "Sending Email",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "c9973266-af63-4837-acc8-6701497e5cc6",
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
              "id": "fd406cc4-2349-4663-a6fb-a51599d6396a"
            }
          ]
        },
        {
          "id": "490948c9-b15a-4feb-9ab2-c9e683d9e3a1",
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
              "id": "939aa491-3fc2-4346-8c35-3a5e0927af81"
            }
          ]
        },
        {
          "id": "45b696a2-eb80-4b31-9408-2bb225ed9c11",
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
              "id": "d52d3198-8b54-4328-86ee-ea3e23b96dac"
            }
          ]
        },
        {
          "id": "176f2eff-e407-4bdb-95a3-5c2161146d22",
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
              "id": "652f8d94-b5b5-49dc-975e-d8b6c2f0f84e"
            }
          ]
        },
        {
          "id": "cd18850d-c85c-4de4-95b6-b03097dd3d52",
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
              "id": "46f0c6b4-7c73-4f3e-8a82-e74232d1f5d4"
            }
          ]
        },
        {
          "id": "da785cd9-e1f5-432e-a1e5-0ffb772a573c",
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
              "id": "79bb0f1a-0627-4ca0-89d0-b22d297176b2"
            }
          ]
        },
        {
          "id": "759e1ed0-d7e0-4c58-954d-f3f7a2501720",
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
              "id": "160a2806-0c2d-4d34-8a5b-21409815111f"
            }
          ]
        },
        {
          "id": "a46dc70a-d060-45f8-b625-713b033b0ea6",
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
              "id": "2fca3dda-823a-41fc-9c87-4bc76eb82e3b"
            }
          ]
        },
        {
          "id": "3926b0a2-85b9-4f85-b488-38b08e0a37aa",
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
              "id": "330de185-3929-49cc-9508-15dadaf22b8c"
            }
          ]
        },
        {
          "id": "bad92c05-03ad-42cc-9f6b-ed6f9e62d574",
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
              "id": "9e8b2b5d-c670-48aa-aaf5-3a04a0e8e483"
            }
          ]
        },
        {
          "id": "dc073bab-01c7-4a62-ad83-6efd64b2f8be",
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
              "id": "95262562-94a7-4343-a745-58964e7d85a0"
            }
          ]
        },
        {
          "id": "80a94c6b-4821-437c-ac7b-9a8b09a41eed",
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
              "id": "50aba644-62e9-47d5-b0f8-756f47f77089"
            }
          ]
        },
        {
          "id": "95ec92e4-db4d-4a94-b394-e08d69b26f4a",
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
              "id": "5ac83e24-1173-4e03-acb5-bd2c7de2237a"
            }
          ]
        },
        {
          "id": "15adc92a-2580-401c-a952-9d6d74c6940f",
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
              "id": "5e85d751-86f5-44fe-bb2b-61b72f49a25f"
            }
          ]
        },
        {
          "id": "55594251-870f-4c9f-a2a4-a4f0088e75f0",
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
              "id": "4e73c96a-4572-4ab9-a1a5-0f50cee41161"
            }
          ]
        }
      ]
    },
    {
      "name": "Updating.Email",
      "item": [
        {
          "id": "776776c6-ec4b-471f-8ac1-538b9bd82f04",
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
              "id": "c681f9be-bc06-4ccd-b9d4-047b3d23f937"
            }
          ]
        }
      ]
    },
    {
      "name": "Create.Email",
      "item": [
        {
          "id": "4ac826ed-aaa4-4cbe-ac37-9d025c6d5751",
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
              "id": "49b1d76b-04c9-4d45-9ff7-7a2668ea2d54"
            }
          ]
        }
      ]
    },
    {
      "name": "Deleting.Email",
      "item": [
        {
          "id": "1920e94d-f7ea-4d92-9a4a-53645c37fba2",
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
              "id": "cf0bf7ea-3b99-40a5-bf29-90386cdc78b3"
            }
          ]
        }
      ]
    },
    {
      "name": ".Email",
      "item": [
        {
          "id": "f2d736cd-5367-48fe-b5ce-1dd0bdda115f",
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
              "id": "d1db7eb8-0b5f-48c1-a903-a1d10b2385dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Activate",
      "item": [
        {
          "id": "e3f3f808-aa58-4640-9c5f-bdeb0247c5fc",
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
              "id": "673aa4dd-c347-4577-b0cf-c0dacf0c0193"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "ee58025c-1dac-4cf2-87ca-ec0869975463",
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
              "id": "82f9fa73-423e-4001-820b-641faacb89a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique",
      "item": [
        {
          "id": "18f27759-a34b-45f1-86fb-b37361d5e3ee",
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
              "id": "a448f633-82d5-46d1-a940-95df926dfbd3"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "27e2cc70-d25a-4ff8-8d71-eff41a951168",
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
              "id": "c6864378-1237-4142-b331-456949c0523f"
            }
          ]
        }
      ]
    }
  ]
}