---
title: "Read MailMerge Document Field Names"
type: docs
url: /read-mailmerge-document-field-names/
aliases: [/read-mailmerge-document-field-names/]
keywords: "Read, mustache template, online, Mail Merge, Word, Microsoft Word, Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "In this article you will learn that how to get MailMerge Field Names in the document in various languages. You can download the SDK of your favorite language and start programming. The SDKs are available in Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android and Go languages."
weight: 30
---

This example explains how to get MailMerge Field Names in the document. Description of some important parameters of the API is given below:

- **useNonMergeFields:** Result includes "mustache" field names if UseNonMergeFields is true

**Note:** The SDKs are available in Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android and Go languages.

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/MailMerge/GetDocumentFieldNamesOnline) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to read MailMerge document Field Names
curl -v "https://api.aspose.cloud/v4.0/words/SampleMailMergeTemplate.docx/mailMerge/FieldNames" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
    "FieldNames": {
        "Names": [
            "FullName",
            "Company",
            "Address",
            "Address2",
            "City",
            "FullName"

        ],
        "link": {
            "Href": "http://api.aspose.cloud/v4.0/words/SampleMailMergeTemplate.docx/mailmerge/getFieldNames",
            "Rel": "self",
            "Type": null,
            "Title": null
        }
    },
    "Code": 200,
    "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetDocumentFieldNames.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentFieldNames.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "GetDocumentFieldNames.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetDocumentFieldNames.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetDocumentFieldNames.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetDocumentFieldNames.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentFieldNames.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentFieldNames.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentFieldNames.go" >}}
{{< /tab >}}
{{< /tabs >}}