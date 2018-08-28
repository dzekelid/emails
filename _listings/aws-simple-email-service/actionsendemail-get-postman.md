{
  "info": {
    "name": "AWS Simple Email Service API Send Email",
    "_postman_id": "c884a767-3057-451c-a074-0e5d38d62144",
    "description": "Composes an email message based on input data, and then immediately queues the message for sending.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "a6685b77-f4b8-4785-833a-843d59e8e082",
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
              "id": "557fe7c5-922a-444e-ac47-540575ae2a44"
            }
          ]
        },
        {
          "id": "790c9d82-f025-4284-bdc7-64183b9c8eb7",
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
              "id": "8cdba88f-5218-4bb1-90f6-bad5565bab7a"
            }
          ]
        },
        {
          "id": "4b9b8c6f-71eb-49cf-9596-cc4ec9d293bb",
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
              "id": "ae1f9310-6fcb-4446-953e-3a58e7b9bbb7"
            }
          ]
        },
        {
          "id": "fd6fbf3d-52f0-4a9f-91d7-889df81b653e",
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
              "id": "5cf36d03-9b59-4c80-b323-92ed1382d989"
            }
          ]
        },
        {
          "id": "f2e4a37f-4fff-4953-92c7-1979e673f3f4",
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
              "id": "d66b3a7a-e97d-4e0b-86d2-4ae973d69db7"
            }
          ]
        },
        {
          "id": "f879e5ea-c0a3-4ebc-9c13-79650d4fb97c",
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
              "id": "ba42b1e4-1214-4f2d-90fa-79852a7b9a69"
            }
          ]
        },
        {
          "id": "408af41b-69bc-4044-8746-5d74bd2bcb40",
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
              "id": "5619c167-6433-4ef2-b715-334fc8a19b7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "07887c33-464b-4431-9fff-7de67b31bc90",
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
              "id": "ee5cc0aa-d7a3-47c2-9f59-04fad8310cb3"
            }
          ]
        },
        {
          "id": "ffab41d7-74a8-44da-bf9a-d5ed6a413b2c",
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
              "id": "8ef80caf-e2f0-4ac7-83f0-b4eb107394c3"
            }
          ]
        },
        {
          "id": "10ef6a59-6fa4-4699-a2e4-3d5ba8b9916b",
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
              "id": "72e00e3d-27d7-4ca8-a389-1a25af7621bd"
            }
          ]
        },
        {
          "id": "19efdc6b-f3db-43da-9f41-ebebc132fb17",
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
              "id": "f3c56946-0431-4223-bc80-fb31b1cbb3be"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "261587cd-8803-4886-988c-e056e6f94141",
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
              "id": "f19ca7b5-e805-44f8-8bc8-713db76dc050"
            }
          ]
        },
        {
          "id": "9da64f9f-1933-4185-85fa-47c2b07da201",
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
              "id": "2c6038cd-112f-4e1d-bb90-a5ce4e0f1eb0"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "cbed666d-b3ca-4487-8c6a-804506af9460",
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
              "id": "55b5aba6-b3ff-4035-9279-ccc68d4770c4"
            }
          ]
        },
        {
          "id": "3a0a6fa4-a78b-4ad7-a51b-9b8198aaa0c1",
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
              "id": "d08a09f1-e107-4d8e-92fc-5aa1676e8417"
            }
          ]
        },
        {
          "id": "171a0794-851e-4a5b-be66-02c6b4e15450",
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
              "id": "dfd39cf6-f8fc-44d9-9978-9b8491e818fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "0fbe6c96-ed20-4f5d-8b3b-425fd07dedbf",
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
              "id": "85322d4f-ec08-4b91-8149-d3213eabc08a"
            }
          ]
        },
        {
          "id": "3ddae117-42a5-4075-87ec-f6696f21e823",
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
              "id": "102cb6a3-0973-4c03-9018-ce3b89951af2"
            }
          ]
        },
        {
          "id": "06a7058b-e345-4d87-b812-459679f1fee1",
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
              "id": "5c45b655-ca51-4853-82de-62458c4775c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "dd83824a-9cdd-46a0-acbd-8e5688c6f19c",
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
              "id": "9f9b814c-3e64-44f6-80ec-ec2cdd1ca285"
            }
          ]
        },
        {
          "id": "15834fbc-c412-4f07-96dd-6d3040b80625",
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
              "id": "0c3b8bc8-5186-4cd2-a7d5-99889cfd2bdd"
            }
          ]
        },
        {
          "id": "cec3b179-6be6-44fe-a769-1d445f426559",
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
              "id": "e5513ce6-96c6-439b-94a1-900b263786f7"
            }
          ]
        },
        {
          "id": "3c48abd9-0eb3-4a45-aad8-01f898e52e2c",
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
              "id": "5d5180b6-54e3-4b53-9d04-efcb9a6f77cc"
            }
          ]
        },
        {
          "id": "a9e4ebc2-fd26-4d85-9762-0744cc97dcdd",
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
              "id": "992be95a-4d19-4ecd-b330-9edd0e1a3044"
            }
          ]
        },
        {
          "id": "af47c6b6-df6e-4736-b1ca-9a4974c22ca2",
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
              "id": "4dce3be0-d9a6-47d9-944d-14dda4b88a54"
            }
          ]
        },
        {
          "id": "73dc2422-31f6-45d0-91b6-de0990e64995",
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
              "id": "619adfc8-6606-43a9-a23b-aa285d474ef0"
            }
          ]
        },
        {
          "id": "1057cf1c-c906-40c6-b65d-275a7b98a235",
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
              "id": "d45ca18e-2aaf-4f41-8108-629067fbe355"
            }
          ]
        },
        {
          "id": "270b6289-c559-4941-8a94-37ec7e609d47",
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
              "id": "9d8ccc18-6c53-4573-ae0b-93ef2e7436dc"
            }
          ]
        },
        {
          "id": "e94c3c62-64e1-4dd4-9562-ae5e2d752377",
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
              "id": "b2dd1ffd-1516-4658-9455-7b0aadb536df"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "e7f6589a-6cb8-4b79-9b3b-9834cb6beeb0",
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
              "id": "b728907d-03a1-4dff-b6d0-8062c55ac902"
            }
          ]
        },
        {
          "id": "15c1856c-6cc8-44a5-a670-1373b2f48365",
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
              "id": "2fa678fb-245b-43a8-a0e9-97b0608059bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "bd3a6594-6879-456c-8d9b-5485f96319e6",
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
              "id": "f8b83c90-20e1-442e-a311-0387ba7c3e95"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "582e724b-5bb8-433e-8208-611559a714fd",
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
              "id": "e45acb17-5c14-4abc-8420-c5cbce0b78c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "59002b45-c132-4a74-9adf-5efdc589840f",
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
              "id": "da4d36d5-80fb-4d04-b2e2-f7d2cf6974a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Email",
      "item": [
        {
          "id": "69d9e434-bf84-4473-93b5-8c26abb77f07",
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
              "id": "a4ca7802-0473-424b-9639-3ee548755224"
            }
          ]
        }
      ]
    }
  ]
}