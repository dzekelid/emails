{
  "info": {
    "name": "Dyn Retrieve Email Bounces",
    "_postman_id": "7c02dc87-319d-4ce5-8a43-e9e96129bcfb",
    "description": "Retrieving the Email SPAM Complaints",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "f4338773-bdab-4223-954c-077f530c928d",
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
              "id": "8dfc1011-56cd-48e1-b4a2-351d8dbf4104"
            }
          ]
        },
        {
          "id": "2d87241e-0ec3-404e-8955-316a84194619",
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
              "id": "3a71949a-5976-41cc-8bd6-f8bd20eef86f"
            }
          ]
        },
        {
          "id": "993b7eb0-49f6-48c8-9326-acb1894a3ec3",
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
              "id": "4589a5a6-5ae9-4e8b-93fd-f92cc1426c67"
            }
          ]
        }
      ]
    },
    {
      "name": "Updating.Email",
      "item": [
        {
          "id": "75925ce2-57a4-4442-9003-0a9d4dd6c14f",
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
              "id": "8084bd47-412d-4021-bd8b-9c835062b7be"
            }
          ]
        }
      ]
    },
    {
      "name": "Create.Email",
      "item": [
        {
          "id": "a79bf4a4-53e6-4250-926c-91cd0ee856a2",
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
              "id": "b3f4174a-9c6e-48ef-ada7-61b8a3b7d313"
            }
          ]
        }
      ]
    },
    {
      "name": "Deleting.Email",
      "item": [
        {
          "id": "411ab0cc-66b2-46c4-bbbd-dae6e1e92270",
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
              "id": "68a321ea-50cb-4809-9b08-0e68f86eaaaf"
            }
          ]
        }
      ]
    },
    {
      "name": ".Email",
      "item": [
        {
          "id": "4321966c-e090-4ebf-b1d3-543b165befe2",
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
              "id": "0d362ecb-5d70-40ac-a5a4-5be13d5aaf12"
            }
          ]
        }
      ]
    },
    {
      "name": "Activate",
      "item": [
        {
          "id": "5efc7d3b-4337-4c07-adb3-16e870dfad9a",
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
              "id": "c5ac76d3-34fe-4440-a7d3-288498172b42"
            }
          ]
        }
      ]
    }
  ]
}