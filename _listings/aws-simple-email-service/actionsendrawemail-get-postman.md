{
  "info": {
    "name": "AWS Simple Email Service API Send Raw Email",
    "_postman_id": "b2b3a108-228d-47be-97cd-2591af765c62",
    "description": "Sends an email message, with header and content specified by the client.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "9c750a8d-f142-4334-82f1-d9a82593602c",
          "name": "cloneReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CloneReceiptRuleSet?OriginalRuleSetName=OriginalRuleSetName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule set by cloning an existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf26bdbf-7960-4ae5-8231-2bdf3a8903ab"
            }
          ]
        },
        {
          "id": "b75e2531-1ba8-4280-a303-8fc7d857ba3a",
          "name": "createReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6a23bd3-dce1-49ea-b0c2-df1e0b5fd786"
            }
          ]
        },
        {
          "id": "51338179-80f1-478e-b9f2-bb92a1da173c",
          "name": "deleteReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule set and all of the receipt rules it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed3f4284-4ed2-4d8b-92c9-2275b8885bee"
            }
          ]
        },
        {
          "id": "2423f305-58e1-4325-aa9e-64d092a6c99c",
          "name": "describeActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActiveReceiptRuleSet?Metadata=Metadata&Rules.member.N=Rules.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata and receipt rules for the receipt rule set that is currently active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1243fee7-a44e-437d-9392-86ca3230f38b"
            }
          ]
        },
        {
          "id": "61f1e362-d373-4773-9b01-e700e3883c47",
          "name": "describeReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cadef03c-e450-48e5-af15-2e05de39b939"
            }
          ]
        },
        {
          "id": "b53046d9-5bd1-4715-8074-90280c108583",
          "name": "listReceiptRuleSets",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptRuleSets?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the receipt rule sets that exist under your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3197ca4-12cb-4ba9-82b7-5b6bba696f17"
            }
          ]
        },
        {
          "id": "87d1f1a8-1c57-4f6a-93f8-861c10854098",
          "name": "reorderReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=ReorderReceiptRuleSet?RuleNames.member.N=RuleNames.member.N&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reorders the receipt rules within a receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c04105d-7f8d-4790-bee0-f88c48761f96"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "1961107c-5350-4046-b9c2-d6a5a8be7c36",
          "name": "createConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSet?ConfigurationSet=ConfigurationSet",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee7139f1-61f9-4b7d-9e10-5ec66a9ff35e"
            }
          ]
        },
        {
          "id": "c8d57a7e-c3dc-49fc-a7b8-11f26d523bbb",
          "name": "deleteConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSet?ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f637870-90ad-40f6-b57e-16f622f84e50"
            }
          ]
        },
        {
          "id": "4d0571a5-682a-4a84-a223-3de74109103d",
          "name": "describeConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationSet?ConfigurationSetAttributeNames.member.N=ConfigurationSetAttributeNames.member.N&ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29071413-3f0e-4a2c-b271-f9b9e14ee2a4"
            }
          ]
        },
        {
          "id": "a84ea163-5225-4836-8c96-7100c5601689",
          "name": "listConfigurationSets",
          "request": {
            "url": "http://example.com/api/?Action=ListConfigurationSets?MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the configuration sets associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9d591ad-39c5-41c1-9ebc-436eea7e74af"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "d808b3b4-1eb1-4242-b2ca-df192b88b8e6",
          "name": "createConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestination=EventDestination",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebf83bb0-4319-4513-9f85-488a965b0c5f"
            }
          ]
        },
        {
          "id": "8c229ba7-1517-4e20-9c83-77a93abc4d85",
          "name": "deleteConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestinationName=EventDestinationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5912a368-1566-429b-a29c-9fa63896a779"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "75d6d010-ea25-40b2-97e4-f40522e16f53",
          "name": "createReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptFilter?Filter=Filter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cc91ad4-b0a7-41e1-b998-c48266e3158f"
            }
          ]
        },
        {
          "id": "3f41d522-b5fc-4a09-992e-f1dedc3696a2",
          "name": "deleteReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptFilter?FilterName=FilterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33ad02d5-aa6d-4aec-afe9-3523a3359eac"
            }
          ]
        },
        {
          "id": "8d39b438-ee77-4464-8553-e7ead44d956e",
          "name": "listReceiptFilters",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptFilters?Filters.member.N=Filters.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IP address filters associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f75ba62d-3c10-488a-9b8b-38c3369a7613"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "4326b4b8-a968-4ae9-93c0-e2b9364eda19",
          "name": "createReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRule?After=After&Rule=Rule&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6401d762-6035-4f5c-804c-d5a9ab217469"
            }
          ]
        },
        {
          "id": "29c07a56-7773-48be-9860-b07a6604e94d",
          "name": "deleteReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7db04d45-d26a-4d6c-8176-d8f3263a8e43"
            }
          ]
        },
        {
          "id": "1f69f7cd-d410-4096-a035-ace0f87390f1",
          "name": "describeReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68f3894b-c22c-419b-bd65-2bca60f3af44"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "6ae3fcc0-053d-4095-bcc2-a0e7d8546416",
          "name": "deleteIdentity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentity?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified identity (an email address or a domain) from the list of verified identities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f2b130c-745e-4a37-a8d6-ea5be231eff6"
            }
          ]
        },
        {
          "id": "704f3cea-76be-46fa-a0c6-a0648f5d0a8e",
          "name": "deleteIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentityPolicy?Identity=Identity&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified sending authorization policy for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e608a3bf-1248-4b15-8678-ef4ee6113aa7"
            }
          ]
        },
        {
          "id": "ee626e27-bf94-4592-8e97-19c5554b7f52",
          "name": "getIdentityDkimAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityDkimAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current status of Easy DKIM signing for an entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd7dabc5-ad9d-4649-a8d2-a7f96f89658e"
            }
          ]
        },
        {
          "id": "e422a5cd-4db6-4e4e-b233-14d829740c68",
          "name": "getIdentityMailFromDomainAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityMailFromDomainAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the custom MAIL FROM attributes for a list of identities (email addresses and/or domains)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8453a598-3d1d-49a3-9d1e-478ccf5d7f82"
            }
          ]
        },
        {
          "id": "6b5f25e1-956b-4d57-97c6-d5605892ac85",
          "name": "getIdentityNotificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityNotificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of verified identities (email addresses and/or domains), returns a structure describing identity notification attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7179fb96-0bcd-481b-952f-fe535cb7f0ad"
            }
          ]
        },
        {
          "id": "4ded089a-50bd-4407-b1e3-ec2b4a599eb6",
          "name": "getIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPolicies?Identity=Identity&PolicyNames.member.N=PolicyNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the requested sending authorization policies for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b72512e-22eb-48fd-8669-6979edd78d1b"
            }
          ]
        },
        {
          "id": "7d65d18b-5133-4887-8c49-4cd8152d5597",
          "name": "getIdentityVerificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityVerificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of identities (email addresses and/or domains), returns the verification status and (for domain identities) the verification token for each identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a60a8c84-cede-4f00-b581-11e4bb8c39aa"
            }
          ]
        },
        {
          "id": "12128c1a-4dcc-41c5-93c0-456902f09d11",
          "name": "listIdentities",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentities?IdentityType=IdentityType&MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the identities (email addresses and domains) for your AWS account, regardless of verification status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17edf8dd-a985-4e6d-a047-f6e218dadcde"
            }
          ]
        },
        {
          "id": "983b16c1-fa8b-46aa-a57f-42161e598e37",
          "name": "listIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPolicies?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of sending authorization policies that are attached to the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e08666e-4dc3-4607-b26e-cb0fd699be09"
            }
          ]
        },
        {
          "id": "7c3f8950-f3e9-4b89-8419-5beb3bd562a3",
          "name": "putIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutIdentityPolicy?Identity=Identity&Policy=Policy&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or updates a sending authorization policy for the specified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5545bb13-9d96-4e75-8458-0ebe2b4cb7be"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "240fa88a-9b0d-4d2d-9ab8-71a4fd93f9a9",
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
              "id": "fda01f46-f69e-479b-9650-e1fc8937ac76"
            }
          ]
        },
        {
          "id": "9bdcedd3-b660-46c6-bf9a-6cf6b0924627",
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
              "id": "766f94c5-ac00-464b-94f6-975b343be7e7"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "afb8997a-587c-4584-b4d9-66a9fc13b1cc",
          "name": "getSendQuota",
          "request": {
            "url": "http://example.com/api/?Action=GetSendQuota?Max24HourSend=Max24HourSend&MaxSendRate=MaxSendRate&SentLast24Hours=SentLast24Hours",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's current sending limits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ee0d4bd-5863-4064-8376-0eea9d75d33d"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "c2f27d85-73a3-4c4f-8751-d0a459c907d7",
          "name": "getSendStatistics",
          "request": {
            "url": "http://example.com/api/?Action=GetSendStatistics?SendDataPoints.member.N=SendDataPoints.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's sending statistics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fd0ba24-c47e-4a4f-9b2d-df94ddb9dc70"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "b7e3a85d-72c3-4e04-a32a-e33f9cc34f60",
          "name": "sendBounce",
          "request": {
            "url": "http://example.com/api/?Action=SendBounce?BouncedRecipientInfoList.member.N=BouncedRecipientInfoList.member.N&BounceSender=BounceSender&BounceSenderArn=BounceSenderArn&Explanation=Explanation&MessageDsn=MessageDsn&OriginalMessageId=OriginalMessageId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates and sends a bounce message to the sender of an email you received through Amazon SES."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2239bc9f-b16b-457d-8346-03253f9c7eb7"
            }
          ]
        }
      ]
    },
    {
      "name": "Email",
      "item": [
        {
          "id": "0db02b54-255e-48c9-9595-a52f8d810b4f",
          "name": "sendEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendEmail?ConfigurationSetName=ConfigurationSetName&Destination=Destination&Message=Message&ReplyToAddresses.member.N=ReplyToAddresses.member.N&ReturnPath=ReturnPath&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Composes an email message based on input data, and then immediately queues the message for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5a729cb-0f3a-4b8b-9979-fe0a673ccc65"
            }
          ]
        },
        {
          "id": "b31c59bd-2c04-4ef0-b27b-2d7cfc680e0d",
          "name": "sendRawEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendRawEmail?ConfigurationSetName=ConfigurationSetName&Destinations.member.N=Destinations.member.N&FromArn=FromArn&RawMessage=RawMessage&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends an email message, with header and content specified by the client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad10db18-4d13-4476-b389-afa1e369cbd7"
            }
          ]
        }
      ]
    }
  ]
}