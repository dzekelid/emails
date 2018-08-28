---
name: Postmark
x-slug: postmark
description: Trusted by thousands of developers, Postmark is a fast and reliable transactional
  email service. Send with Postmark to ensure your transactional emails get to the
  inbox on time, every time.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
x-kinRank: "8"
x-alexaRank: "87545"
tags: Emails
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/apis.md
specificationVersion: "0.14"
apis:
- name: Postmark - Parameters Email
  x-api-slug: email-parameters
  description: Parameters email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-openapi.md
- name: Postmark - Post Email
  x-api-slug: email-post
  description: |-
    Sends e-mails. Currently Postmark supports JSON message format. The mail message format is:

    {
        "From" : "sender@example.com",
        "To" : "receiver@example.com",
        "Cc" : "copied@example.com",
        "Bcc": "blank-copied@example.com",
        "Subject" : "Test",
        "Tag" : "Invitation",
        "HtmlBody" : "Hello",
        "TextBody" : "Hello",
        "ReplyTo" : "reply@example.com",
        "Headers" : [{ "Name" : "CUSTOM-HEADER", "Value" : "value" }],
        "Attachments": [
            {
                 "Name": "readme.txt",
                 "Content": "dGVzdCBjb250ZW50",
                 "ContentType": "text/plain"
            },
            {
                "Name": "report.pdf",
                "Content": "dGVzdCBjb250ZW50",
                "ContentType": "application/octet-stream"
            }
        ]
    }

    You should pass the json encoded message in the body of the request. Both from and to accept name, in the format of John Doe . You can provide HtmlBody for html formatted messages, TextBody for plain text, or both for multipart. Multipart sends html with a text version for clients that don???t support html. Passing headers is optional.

    1. You should have a registered and confirmed sender signature with the sender email. Otherwise you will receive HTTP Response 422 (Unprocessable Entity).
    2. It is possible to override the Name in the sender signature through the API. This is useful if you want to use member???s information in the email while keeping your from email address. just pass the name in the From parameter, From: "John Smith ".
    3. You can pass multiple recipient addresses in the ???To??? field and the optional ???Cc??? and ???Bcc??? fields. Separate multiple addresses with a comma. Note that Postmark has a limit of twenty recipients per message in total. You need to take care not to exceed that limit. Otherwise you will get an error.
    4. You can categorize outgoing email using the optional Tag property. If you use different tags for the different types of emails your application generates, you will be able to get detailed statistics for them through the Postmark user interface.

    Attachments
    Attachments are specified in the Attachments array property. An attachment is an object that has to provide the file name (via the Name property), the content type (ContentType property) and the actual binary data (Content property) that has to be sent with the message.

    The name is the actual file name that will be displayed to the message recipient. Note that the file extension is important. To eliminate the possibility of spreading viruses or spyware we allow only a number of file types. That is, instead of using a list of forbidden files and risking an unanticipated file type spreading infections, we have taken the opposite approach ??? we whitelist document file types that we are certain are safe. Here is the list of allowed files:

    - Media files: gif, jpg, jpeg, png, swf, flv, avi, mpg, mp3, mp4, ogv, wav, rm, mov, psd, ai, tif, tiff
    - Documents: txt, rtf, htm, html, pdf, epub, mobi, doc, docx, ppt, pptx, xls, xlsx, ps, eps, iif
    - Miscellaneous: log, csv, ics, xml, zip

    Contact us if you feel we need to whitelist a file that your application needs.

    The content type is the MIME content type that email clients use to interpret various attachments such as: text/plain, text/html, image/jpeg, etc. Your code can either detect it by the file extension, use a third party library to infer it, ask the user to provide it or just default to application/octet-stream.

    The binary data has to be transmitted as a base64-encoded string. Most programming languages and libraries have this built in e.g. Java, .NET, PHP, Ruby.

    You can use SSL encryption by issuing requests to https://api.postmarkapp.com/email.

    Success
    If all goes well, you will get back a JSON message looking a lot like:

    {
        "ErrorCode" : 0,
        "Message" : "OK",
        "MessageID" : "b7bc2f4a-e38e-4336-af7d-e6c392c2f817",
        "SubmittedAt" : "2010-11-26T12:01:05.1794748-05:00",
        "To" : "receiver@example.com"
    }

    Note the MessageID property. You can log it in your system and use it to associate the message you just sent to a possible bounce that you obtained from a bounce web hook or the bounce API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-post-openapi.md
- name: Postmark - Parameters Email Batch
  x-api-slug: emailbatch-parameters
  description: Parameters email batch.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-openapi.md
- name: Postmark - Post Email Batch
  x-api-slug: emailbatch-post
  description: "While Postmark is focused on transactional email, we understand that
    developers with higher volumes or processing time constraints need to send their
    messages in batches. To facilitate this we provide a batching endpoint that permits
    you to send up to 500 well-formed Postmark messages in a single API call.\n                    \nThe
    format of the batched message is a JSON array containing multiple message requests
    like the following example:\n[\n    {From: 'sender@example.com', To: 'receiver1@example.com',
    Subject: 'Postmark test #1', HtmlBody: 'Hello dear Postmark user.'},\n    {From:
    'sender@example.com', To: 'receiver2@example.com', Subject: 'Postmark test #2',
    HtmlBody: 'Hello dear Postmark user.'}\n]\n\nYou can use SSL encryption by issuing
    requests to https://api.postmarkapp.com/email/batch.\n\nSimilarly, you will receive
    a matching JSON array containing each response for the messages you sent in your
    batched call:\n\n[\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n
    \       \"MessageID\" : \"b7bc2f4a-e38e-4336-af7d-e6c392c2f817\",\n        \"SubmittedAt\"
    : \"2010-11-26T12:01:05.1794748-05:00\",\n        \"To\" : \"receiver1@example.com\"\n
    \   },\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n        \"MessageID\"
    : \"e2ecbbfc-fe12-463d-b933-9fe22915106d\",\n        \"SubmittedAt\" : \"2010-11-26T12:01:05.1794748-05:00\",\n
    \       \"To\" : \"receiver2@example.com\"\n    },\n]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-post-openapi.md
- name: Postmark - Post Email Withtemplate
  x-api-slug: emailwithtemplate-post
  description: Post email withtemplate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailwithtemplate-post-openapi.md
- name: Postmark - Get Stats Outbound Opens Emailclients
  x-api-slug: statsoutboundopensemailclients-get
  description: Get stats outbound opens emailclients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/statsoutboundopensemailclients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/statsoutboundopensemailclients-get-openapi.md
- name: Postmark - Parameters Email
  x-api-slug: email-parameters
  description: Parameters email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-openapi.md
- name: Postmark - Parameters Email
  x-api-slug: email-parameters
  description: Parameters email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-openapi.md
- name: Postmark - Post Email
  x-api-slug: email-post
  description: |-
    Sends e-mails. Currently Postmark supports JSON message format. The mail message format is:

    {
        "From" : "sender@example.com",
        "To" : "receiver@example.com",
        "Cc" : "copied@example.com",
        "Bcc": "blank-copied@example.com",
        "Subject" : "Test",
        "Tag" : "Invitation",
        "HtmlBody" : "Hello",
        "TextBody" : "Hello",
        "ReplyTo" : "reply@example.com",
        "Headers" : [{ "Name" : "CUSTOM-HEADER", "Value" : "value" }],
        "Attachments": [
            {
                 "Name": "readme.txt",
                 "Content": "dGVzdCBjb250ZW50",
                 "ContentType": "text/plain"
            },
            {
                "Name": "report.pdf",
                "Content": "dGVzdCBjb250ZW50",
                "ContentType": "application/octet-stream"
            }
        ]
    }

    You should pass the json encoded message in the body of the request. Both from and to accept name, in the format of John Doe . You can provide HtmlBody for html formatted messages, TextBody for plain text, or both for multipart. Multipart sends html with a text version for clients that don???t support html. Passing headers is optional.

    1. You should have a registered and confirmed sender signature with the sender email. Otherwise you will receive HTTP Response 422 (Unprocessable Entity).
    2. It is possible to override the Name in the sender signature through the API. This is useful if you want to use member???s information in the email while keeping your from email address. just pass the name in the From parameter, From: "John Smith ".
    3. You can pass multiple recipient addresses in the ???To??? field and the optional ???Cc??? and ???Bcc??? fields. Separate multiple addresses with a comma. Note that Postmark has a limit of twenty recipients per message in total. You need to take care not to exceed that limit. Otherwise you will get an error.
    4. You can categorize outgoing email using the optional Tag property. If you use different tags for the different types of emails your application generates, you will be able to get detailed statistics for them through the Postmark user interface.

    Attachments
    Attachments are specified in the Attachments array property. An attachment is an object that has to provide the file name (via the Name property), the content type (ContentType property) and the actual binary data (Content property) that has to be sent with the message.

    The name is the actual file name that will be displayed to the message recipient. Note that the file extension is important. To eliminate the possibility of spreading viruses or spyware we allow only a number of file types. That is, instead of using a list of forbidden files and risking an unanticipated file type spreading infections, we have taken the opposite approach ??? we whitelist document file types that we are certain are safe. Here is the list of allowed files:

    - Media files: gif, jpg, jpeg, png, swf, flv, avi, mpg, mp3, mp4, ogv, wav, rm, mov, psd, ai, tif, tiff
    - Documents: txt, rtf, htm, html, pdf, epub, mobi, doc, docx, ppt, pptx, xls, xlsx, ps, eps, iif
    - Miscellaneous: log, csv, ics, xml, zip

    Contact us if you feel we need to whitelist a file that your application needs.

    The content type is the MIME content type that email clients use to interpret various attachments such as: text/plain, text/html, image/jpeg, etc. Your code can either detect it by the file extension, use a third party library to infer it, ask the user to provide it or just default to application/octet-stream.

    The binary data has to be transmitted as a base64-encoded string. Most programming languages and libraries have this built in e.g. Java, .NET, PHP, Ruby.

    You can use SSL encryption by issuing requests to https://api.postmarkapp.com/email.

    Success
    If all goes well, you will get back a JSON message looking a lot like:

    {
        "ErrorCode" : 0,
        "Message" : "OK",
        "MessageID" : "b7bc2f4a-e38e-4336-af7d-e6c392c2f817",
        "SubmittedAt" : "2010-11-26T12:01:05.1794748-05:00",
        "To" : "receiver@example.com"
    }

    Note the MessageID property. You can log it in your system and use it to associate the message you just sent to a possible bounce that you obtained from a bounce web hook or the bounce API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-post-openapi.md
- name: Postmark - Parameters Email
  x-api-slug: email-parameters
  description: Parameters email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-openapi.md
- name: Postmark - Post Email
  x-api-slug: email-post
  description: |-
    Sends e-mails. Currently Postmark supports JSON message format. The mail message format is:

    {
        "From" : "sender@example.com",
        "To" : "receiver@example.com",
        "Cc" : "copied@example.com",
        "Bcc": "blank-copied@example.com",
        "Subject" : "Test",
        "Tag" : "Invitation",
        "HtmlBody" : "Hello",
        "TextBody" : "Hello",
        "ReplyTo" : "reply@example.com",
        "Headers" : [{ "Name" : "CUSTOM-HEADER", "Value" : "value" }],
        "Attachments": [
            {
                 "Name": "readme.txt",
                 "Content": "dGVzdCBjb250ZW50",
                 "ContentType": "text/plain"
            },
            {
                "Name": "report.pdf",
                "Content": "dGVzdCBjb250ZW50",
                "ContentType": "application/octet-stream"
            }
        ]
    }

    You should pass the json encoded message in the body of the request. Both from and to accept name, in the format of John Doe . You can provide HtmlBody for html formatted messages, TextBody for plain text, or both for multipart. Multipart sends html with a text version for clients that don???t support html. Passing headers is optional.

    1. You should have a registered and confirmed sender signature with the sender email. Otherwise you will receive HTTP Response 422 (Unprocessable Entity).
    2. It is possible to override the Name in the sender signature through the API. This is useful if you want to use member???s information in the email while keeping your from email address. just pass the name in the From parameter, From: "John Smith ".
    3. You can pass multiple recipient addresses in the ???To??? field and the optional ???Cc??? and ???Bcc??? fields. Separate multiple addresses with a comma. Note that Postmark has a limit of twenty recipients per message in total. You need to take care not to exceed that limit. Otherwise you will get an error.
    4. You can categorize outgoing email using the optional Tag property. If you use different tags for the different types of emails your application generates, you will be able to get detailed statistics for them through the Postmark user interface.

    Attachments
    Attachments are specified in the Attachments array property. An attachment is an object that has to provide the file name (via the Name property), the content type (ContentType property) and the actual binary data (Content property) that has to be sent with the message.

    The name is the actual file name that will be displayed to the message recipient. Note that the file extension is important. To eliminate the possibility of spreading viruses or spyware we allow only a number of file types. That is, instead of using a list of forbidden files and risking an unanticipated file type spreading infections, we have taken the opposite approach ??? we whitelist document file types that we are certain are safe. Here is the list of allowed files:

    - Media files: gif, jpg, jpeg, png, swf, flv, avi, mpg, mp3, mp4, ogv, wav, rm, mov, psd, ai, tif, tiff
    - Documents: txt, rtf, htm, html, pdf, epub, mobi, doc, docx, ppt, pptx, xls, xlsx, ps, eps, iif
    - Miscellaneous: log, csv, ics, xml, zip

    Contact us if you feel we need to whitelist a file that your application needs.

    The content type is the MIME content type that email clients use to interpret various attachments such as: text/plain, text/html, image/jpeg, etc. Your code can either detect it by the file extension, use a third party library to infer it, ask the user to provide it or just default to application/octet-stream.

    The binary data has to be transmitted as a base64-encoded string. Most programming languages and libraries have this built in e.g. Java, .NET, PHP, Ruby.

    You can use SSL encryption by issuing requests to https://api.postmarkapp.com/email.

    Success
    If all goes well, you will get back a JSON message looking a lot like:

    {
        "ErrorCode" : 0,
        "Message" : "OK",
        "MessageID" : "b7bc2f4a-e38e-4336-af7d-e6c392c2f817",
        "SubmittedAt" : "2010-11-26T12:01:05.1794748-05:00",
        "To" : "receiver@example.com"
    }

    Note the MessageID property. You can log it in your system and use it to associate the message you just sent to a possible bounce that you obtained from a bounce web hook or the bounce API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-post-openapi.md
- name: Postmark - Parameters Email Batch
  x-api-slug: emailbatch-parameters
  description: Parameters email batch.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-openapi.md
- name: Postmark - Post Email
  x-api-slug: email-post
  description: |-
    Sends e-mails. Currently Postmark supports JSON message format. The mail message format is:

    {
        "From" : "sender@example.com",
        "To" : "receiver@example.com",
        "Cc" : "copied@example.com",
        "Bcc": "blank-copied@example.com",
        "Subject" : "Test",
        "Tag" : "Invitation",
        "HtmlBody" : "Hello",
        "TextBody" : "Hello",
        "ReplyTo" : "reply@example.com",
        "Headers" : [{ "Name" : "CUSTOM-HEADER", "Value" : "value" }],
        "Attachments": [
            {
                 "Name": "readme.txt",
                 "Content": "dGVzdCBjb250ZW50",
                 "ContentType": "text/plain"
            },
            {
                "Name": "report.pdf",
                "Content": "dGVzdCBjb250ZW50",
                "ContentType": "application/octet-stream"
            }
        ]
    }

    You should pass the json encoded message in the body of the request. Both from and to accept name, in the format of John Doe . You can provide HtmlBody for html formatted messages, TextBody for plain text, or both for multipart. Multipart sends html with a text version for clients that don???t support html. Passing headers is optional.

    1. You should have a registered and confirmed sender signature with the sender email. Otherwise you will receive HTTP Response 422 (Unprocessable Entity).
    2. It is possible to override the Name in the sender signature through the API. This is useful if you want to use member???s information in the email while keeping your from email address. just pass the name in the From parameter, From: "John Smith ".
    3. You can pass multiple recipient addresses in the ???To??? field and the optional ???Cc??? and ???Bcc??? fields. Separate multiple addresses with a comma. Note that Postmark has a limit of twenty recipients per message in total. You need to take care not to exceed that limit. Otherwise you will get an error.
    4. You can categorize outgoing email using the optional Tag property. If you use different tags for the different types of emails your application generates, you will be able to get detailed statistics for them through the Postmark user interface.

    Attachments
    Attachments are specified in the Attachments array property. An attachment is an object that has to provide the file name (via the Name property), the content type (ContentType property) and the actual binary data (Content property) that has to be sent with the message.

    The name is the actual file name that will be displayed to the message recipient. Note that the file extension is important. To eliminate the possibility of spreading viruses or spyware we allow only a number of file types. That is, instead of using a list of forbidden files and risking an unanticipated file type spreading infections, we have taken the opposite approach ??? we whitelist document file types that we are certain are safe. Here is the list of allowed files:

    - Media files: gif, jpg, jpeg, png, swf, flv, avi, mpg, mp3, mp4, ogv, wav, rm, mov, psd, ai, tif, tiff
    - Documents: txt, rtf, htm, html, pdf, epub, mobi, doc, docx, ppt, pptx, xls, xlsx, ps, eps, iif
    - Miscellaneous: log, csv, ics, xml, zip

    Contact us if you feel we need to whitelist a file that your application needs.

    The content type is the MIME content type that email clients use to interpret various attachments such as: text/plain, text/html, image/jpeg, etc. Your code can either detect it by the file extension, use a third party library to infer it, ask the user to provide it or just default to application/octet-stream.

    The binary data has to be transmitted as a base64-encoded string. Most programming languages and libraries have this built in e.g. Java, .NET, PHP, Ruby.

    You can use SSL encryption by issuing requests to https://api.postmarkapp.com/email.

    Success
    If all goes well, you will get back a JSON message looking a lot like:

    {
        "ErrorCode" : 0,
        "Message" : "OK",
        "MessageID" : "b7bc2f4a-e38e-4336-af7d-e6c392c2f817",
        "SubmittedAt" : "2010-11-26T12:01:05.1794748-05:00",
        "To" : "receiver@example.com"
    }

    Note the MessageID property. You can log it in your system and use it to associate the message you just sent to a possible bounce that you obtained from a bounce web hook or the bounce API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-post-openapi.md
- name: Postmark - Parameters Email Batch
  x-api-slug: emailbatch-parameters
  description: Parameters email batch.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-openapi.md
- name: Postmark - Post Email Batch
  x-api-slug: emailbatch-post
  description: "While Postmark is focused on transactional email, we understand that
    developers with higher volumes or processing time constraints need to send their
    messages in batches. To facilitate this we provide a batching endpoint that permits
    you to send up to 500 well-formed Postmark messages in a single API call.\n                    \nThe
    format of the batched message is a JSON array containing multiple message requests
    like the following example:\n[\n    {From: 'sender@example.com', To: 'receiver1@example.com',
    Subject: 'Postmark test #1', HtmlBody: 'Hello dear Postmark user.'},\n    {From:
    'sender@example.com', To: 'receiver2@example.com', Subject: 'Postmark test #2',
    HtmlBody: 'Hello dear Postmark user.'}\n]\n\nYou can use SSL encryption by issuing
    requests to https://api.postmarkapp.com/email/batch.\n\nSimilarly, you will receive
    a matching JSON array containing each response for the messages you sent in your
    batched call:\n\n[\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n
    \       \"MessageID\" : \"b7bc2f4a-e38e-4336-af7d-e6c392c2f817\",\n        \"SubmittedAt\"
    : \"2010-11-26T12:01:05.1794748-05:00\",\n        \"To\" : \"receiver1@example.com\"\n
    \   },\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n        \"MessageID\"
    : \"e2ecbbfc-fe12-463d-b933-9fe22915106d\",\n        \"SubmittedAt\" : \"2010-11-26T12:01:05.1794748-05:00\",\n
    \       \"To\" : \"receiver2@example.com\"\n    },\n]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-post-openapi.md
- name: Postmark - Parameters Email Batch
  x-api-slug: emailbatch-parameters
  description: Parameters email batch.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-openapi.md
- name: Postmark - Post Email Batch
  x-api-slug: emailbatch-post
  description: "While Postmark is focused on transactional email, we understand that
    developers with higher volumes or processing time constraints need to send their
    messages in batches. To facilitate this we provide a batching endpoint that permits
    you to send up to 500 well-formed Postmark messages in a single API call.\n                    \nThe
    format of the batched message is a JSON array containing multiple message requests
    like the following example:\n[\n    {From: 'sender@example.com', To: 'receiver1@example.com',
    Subject: 'Postmark test #1', HtmlBody: 'Hello dear Postmark user.'},\n    {From:
    'sender@example.com', To: 'receiver2@example.com', Subject: 'Postmark test #2',
    HtmlBody: 'Hello dear Postmark user.'}\n]\n\nYou can use SSL encryption by issuing
    requests to https://api.postmarkapp.com/email/batch.\n\nSimilarly, you will receive
    a matching JSON array containing each response for the messages you sent in your
    batched call:\n\n[\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n
    \       \"MessageID\" : \"b7bc2f4a-e38e-4336-af7d-e6c392c2f817\",\n        \"SubmittedAt\"
    : \"2010-11-26T12:01:05.1794748-05:00\",\n        \"To\" : \"receiver1@example.com\"\n
    \   },\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n        \"MessageID\"
    : \"e2ecbbfc-fe12-463d-b933-9fe22915106d\",\n        \"SubmittedAt\" : \"2010-11-26T12:01:05.1794748-05:00\",\n
    \       \"To\" : \"receiver2@example.com\"\n    },\n]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-post-openapi.md
- name: Postmark - Post Email Withtemplate
  x-api-slug: emailwithtemplate-post
  description: Post email withtemplate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailwithtemplate-post-openapi.md
- name: Postmark - Post Email Batch
  x-api-slug: emailbatch-post
  description: "While Postmark is focused on transactional email, we understand that
    developers with higher volumes or processing time constraints need to send their
    messages in batches. To facilitate this we provide a batching endpoint that permits
    you to send up to 500 well-formed Postmark messages in a single API call.\n                    \nThe
    format of the batched message is a JSON array containing multiple message requests
    like the following example:\n[\n    {From: 'sender@example.com', To: 'receiver1@example.com',
    Subject: 'Postmark test #1', HtmlBody: 'Hello dear Postmark user.'},\n    {From:
    'sender@example.com', To: 'receiver2@example.com', Subject: 'Postmark test #2',
    HtmlBody: 'Hello dear Postmark user.'}\n]\n\nYou can use SSL encryption by issuing
    requests to https://api.postmarkapp.com/email/batch.\n\nSimilarly, you will receive
    a matching JSON array containing each response for the messages you sent in your
    batched call:\n\n[\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n
    \       \"MessageID\" : \"b7bc2f4a-e38e-4336-af7d-e6c392c2f817\",\n        \"SubmittedAt\"
    : \"2010-11-26T12:01:05.1794748-05:00\",\n        \"To\" : \"receiver1@example.com\"\n
    \   },\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n        \"MessageID\"
    : \"e2ecbbfc-fe12-463d-b933-9fe22915106d\",\n        \"SubmittedAt\" : \"2010-11-26T12:01:05.1794748-05:00\",\n
    \       \"To\" : \"receiver2@example.com\"\n    },\n]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-post-openapi.md
- name: Postmark - Post Email Withtemplate
  x-api-slug: emailwithtemplate-post
  description: Post email withtemplate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailwithtemplate-post-openapi.md
- name: Postmark - Post Email Withtemplate
  x-api-slug: emailwithtemplate-post
  description: Post email withtemplate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailwithtemplate-post-openapi.md
- name: Postmark - Get Stats Outbound Opens Emailclients
  x-api-slug: statsoutboundopensemailclients-get
  description: Get stats outbound opens emailclients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/statsoutboundopensemailclients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/statsoutboundopensemailclients-get-openapi.md
- name: Postmark - Post Email Withtemplate
  x-api-slug: emailwithtemplate-post
  description: Post email withtemplate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailwithtemplate-post-openapi.md
- name: Postmark - Post Email Batch
  x-api-slug: emailbatch-post
  description: "While Postmark is focused on transactional email, we understand that
    developers with higher volumes or processing time constraints need to send their
    messages in batches. To facilitate this we provide a batching endpoint that permits
    you to send up to 500 well-formed Postmark messages in a single API call.\n                    \nThe
    format of the batched message is a JSON array containing multiple message requests
    like the following example:\n[\n    {From: 'sender@example.com', To: 'receiver1@example.com',
    Subject: 'Postmark test #1', HtmlBody: 'Hello dear Postmark user.'},\n    {From:
    'sender@example.com', To: 'receiver2@example.com', Subject: 'Postmark test #2',
    HtmlBody: 'Hello dear Postmark user.'}\n]\n\nYou can use SSL encryption by issuing
    requests to https://api.postmarkapp.com/email/batch.\n\nSimilarly, you will receive
    a matching JSON array containing each response for the messages you sent in your
    batched call:\n\n[\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n
    \       \"MessageID\" : \"b7bc2f4a-e38e-4336-af7d-e6c392c2f817\",\n        \"SubmittedAt\"
    : \"2010-11-26T12:01:05.1794748-05:00\",\n        \"To\" : \"receiver1@example.com\"\n
    \   },\n    {\n        \"ErrorCode\" : 0,\n        \"Message\" : \"OK\",\n        \"MessageID\"
    : \"e2ecbbfc-fe12-463d-b933-9fe22915106d\",\n        \"SubmittedAt\" : \"2010-11-26T12:01:05.1794748-05:00\",\n
    \       \"To\" : \"receiver2@example.com\"\n    },\n]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-post-openapi.md
- name: Postmark - Parameters Email Batch
  x-api-slug: emailbatch-parameters
  description: Parameters email batch.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/emailbatch-parameters-openapi.md
- name: Postmark - Post Email
  x-api-slug: email-post
  description: |-
    Sends e-mails. Currently Postmark supports JSON message format. The mail message format is:

    {
        "From" : "sender@example.com",
        "To" : "receiver@example.com",
        "Cc" : "copied@example.com",
        "Bcc": "blank-copied@example.com",
        "Subject" : "Test",
        "Tag" : "Invitation",
        "HtmlBody" : "Hello",
        "TextBody" : "Hello",
        "ReplyTo" : "reply@example.com",
        "Headers" : [{ "Name" : "CUSTOM-HEADER", "Value" : "value" }],
        "Attachments": [
            {
                 "Name": "readme.txt",
                 "Content": "dGVzdCBjb250ZW50",
                 "ContentType": "text/plain"
            },
            {
                "Name": "report.pdf",
                "Content": "dGVzdCBjb250ZW50",
                "ContentType": "application/octet-stream"
            }
        ]
    }

    You should pass the json encoded message in the body of the request. Both from and to accept name, in the format of John Doe . You can provide HtmlBody for html formatted messages, TextBody for plain text, or both for multipart. Multipart sends html with a text version for clients that don???t support html. Passing headers is optional.

    1. You should have a registered and confirmed sender signature with the sender email. Otherwise you will receive HTTP Response 422 (Unprocessable Entity).
    2. It is possible to override the Name in the sender signature through the API. This is useful if you want to use member???s information in the email while keeping your from email address. just pass the name in the From parameter, From: "John Smith ".
    3. You can pass multiple recipient addresses in the ???To??? field and the optional ???Cc??? and ???Bcc??? fields. Separate multiple addresses with a comma. Note that Postmark has a limit of twenty recipients per message in total. You need to take care not to exceed that limit. Otherwise you will get an error.
    4. You can categorize outgoing email using the optional Tag property. If you use different tags for the different types of emails your application generates, you will be able to get detailed statistics for them through the Postmark user interface.

    Attachments
    Attachments are specified in the Attachments array property. An attachment is an object that has to provide the file name (via the Name property), the content type (ContentType property) and the actual binary data (Content property) that has to be sent with the message.

    The name is the actual file name that will be displayed to the message recipient. Note that the file extension is important. To eliminate the possibility of spreading viruses or spyware we allow only a number of file types. That is, instead of using a list of forbidden files and risking an unanticipated file type spreading infections, we have taken the opposite approach ??? we whitelist document file types that we are certain are safe. Here is the list of allowed files:

    - Media files: gif, jpg, jpeg, png, swf, flv, avi, mpg, mp3, mp4, ogv, wav, rm, mov, psd, ai, tif, tiff
    - Documents: txt, rtf, htm, html, pdf, epub, mobi, doc, docx, ppt, pptx, xls, xlsx, ps, eps, iif
    - Miscellaneous: log, csv, ics, xml, zip

    Contact us if you feel we need to whitelist a file that your application needs.

    The content type is the MIME content type that email clients use to interpret various attachments such as: text/plain, text/html, image/jpeg, etc. Your code can either detect it by the file extension, use a third party library to infer it, ask the user to provide it or just default to application/octet-stream.

    The binary data has to be transmitted as a base64-encoded string. Most programming languages and libraries have this built in e.g. Java, .NET, PHP, Ruby.

    You can use SSL encryption by issuing requests to https://api.postmarkapp.com/email.

    Success
    If all goes well, you will get back a JSON message looking a lot like:

    {
        "ErrorCode" : 0,
        "Message" : "OK",
        "MessageID" : "b7bc2f4a-e38e-4336-af7d-e6c392c2f817",
        "SubmittedAt" : "2010-11-26T12:01:05.1794748-05:00",
        "To" : "receiver@example.com"
    }

    Note the MessageID property. You can log it in your system and use it to associate the message you just sent to a possible bounce that you obtained from a bounce web hook or the bounce API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-post-openapi.md
- name: Postmark - Parameters Email
  x-api-slug: email-parameters
  description: Parameters email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/email-parameters-openapi.md
- name: Postmark - Get Stats Outbound Opens Emailclients
  x-api-slug: statsoutboundopensemailclients-get
  description: Get stats outbound opens emailclients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/statsoutboundopensemailclients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/emails/master/_listings/postmark/statsoutboundopensemailclients-get-openapi.md
x-common:
- type: x--net-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#dot-net
- type: x-api-gallery
  url: http://polygon.api.gallery.streamdata.io
- type: x-api-stack
  url: http://postmark.stack.network
- type: x-base
  url: https://api.postmarkapp.com
- type: x-blog
  url: http://blog.postmarkapp.com/
- type: x-blog-rss
  url: http://blog.postmarkapp.com/rss
- type: x-contact-form
  url: http://support.postmarkapp.com/customer/portal/emails/new
- type: x-crunchbase
  url: https://crunchbase.com/organization/postmark
- type: x-crunchbase
  url: http://www.crunchbase.com/company/postmark
- type: x-developer
  url: http://developer.postmarkapp.com/
- type: x-email
  url: support@postmarkapp.com
- type: x-email
  url: 451d9b70cf9364d23ff6f9d51d870251569e+ahoy@inbound.postmarkapp.com
- type: x-faq
  url: http://support.postmarkapp.com/
- type: x-pricing
  url: http://developer.postmarkapp.com/developer-api-messages.html
- type: x-privacy
  url: https://postmarkapp.com/privacy-policy
- type: x-ruby-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#rails
- type: x-ruby-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#ruby
- type: x-selfservice-registration
  url: https://postmarkapp.com/sign_up
- type: x-status
  url: http://status.postmarkapp.com/
- type: x-terms-of-service
  url: https://postmarkapp.com/terms-of-service
- type: x-twitter
  url: https://twitter.com/postmarkapp
- type: x-website
  url: http://postmarkapp.com
- type: x-website
  url: http://postmarkapp.com/
- type: x-website
  url: https://postmarkapp.com
- type: x-wordpress-pdk
  url: http://developer.postmarkapp.com/developer-official-libs.html#wordpress
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---