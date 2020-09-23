---
title: "Read the Page Setup of a Section"
type: docs
url: /read-the-page-setup-of-a-section/
aliases: [/read-the-page-setup-of-a-section/]
keywords: "page setup word,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to read the page setup of a section. The API returns JSON/XML representation of the section page setup. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift and Go languages."
weight: 30
---

This REST API allows you to read the page setup of a section. The API returns JSON/XML representation of the section page setup. The resource properties are the following:

|Property Name|Type|Description|
| :- | :- | :- |
|Bidi|bool|Specifies that this section contains bidirectional (complex scripts) text.|
|BorderAlwaysInFront|bool|Specifies where the page border is positioned relative to intersecting texts and objects.|
|BorderAppliesTo|PageBorderAppliesTo|Specifies which pages the page border is printed on.|
|BorderDistanceFrom|PageBorderDistanceFrom|Specifies a value that indicates whether the specified page border is measured from the edge of the page or from the text it surrounds.|
|BottomMargin|double|Specifies the distance (in points) between the bottom edge of the page and the bottom boundary of the body text.|
|DifferentFirstPageHeaderFooter|bool|True if a different header or footer is used on the first page.|
|FirstPageTray|int|Specifies the paper tray (bin) to use for the first page of a section. The value is implementation (printer) specific.|
|FooterDistance|double|Specifies the distance (in points) between the footer and the bottom of the page.|
|Gutter|double|Specifies the amount of extra space added to the margin for document binding.|
|HeaderDistance|double|Specifies the distance (in points) between the header and the top of the page.|
|LeftMargin|double|Specifies the distance (in points) between the left edge of the page and the left boundary of the body text.|
|LineNumberCountBy|int|Specifies the numeric increment for line numbers.|
|LineNumberDistanceFromText|double|Specifies the distance between the right edge of line numbers and the left edge of the document. Set this property to zero for the automatic distance between the line numbers and text of the document.|
|LineNumberRestartMode|LineNumberRestartMode|Specifies the way line numbering runs that is, whether it starts over at the beginning of a new page or section or runs continuously.|
|LineStartingNumber|int|Specifies the starting line number.|
|Orientation|Orientation|Specifies the orientation of the page. Changing 'Orientation' swaps 'PageWidth' and 'PageHeight'.|
|OtherPagesTray|int|Specifies the paper tray (bin) to be used for all but the first page of a section. The value is implementation (printer) specific.|
|PageHeight|double|Specifies the height of the page in points.|
|PageNumberStyle|NumberStyle|Specifies the page number format.|
|PageStartingNumber|int|Specifies the starting page number of the section. The 'RestartPageNumbering' property, if set to false, will override the 'PageStartingNumber' property so that page numbering can continue from the previous section.|
|PageWidth|double|Specifies the width of the page in points.|
|PaperSize|PaperSize|Specifies the paper size. Setting this property updates 'PageWidth' and 'PageHeight' values. Setting this value to 'Custom' does not change existing values.|
|RestartPageNumbering|bool|True if page numbering restarts at the beginning of the section. If set to false, the 'RestartPageNumbering' property will override the 'PageStartingNumber' property so that page numbering can continue from the previous section.|
|RightMargin|double|Specifies the distance (in points) between the right edge of the page and the right boundary of the body text.|
|RtlGutter|bool|Specifies whether Microsoft Word uses gutters for the section based on a right-to-left language or a left-to-right language.|
|SectionStart|SectionStart|Specifies the type of section break for the specified object.|
|SuppressEndnotes|bool|True if endnotes are printed at the end of the next section that doesn't suppress endnotes. Suppressed endnotes are printed before the endnotes in that section.|
|TopMargin|double|Specifies the distance (in points) between the top edge of the page and the top boundary of the body text.|
|VerticalAlignment|PageVerticalAlignment|Specifies the vertical alignment of text on each page in a document or section.|
Please note that the SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift* and *Go* languages.

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Sections/GetSectionPageSetup) lets you call this REST API directly from a browser.

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

# cURL example to get setup of section
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pageSetup" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "PageSetup": {
    "Bidi": false,
    "BorderAlwaysInFront": true,
    "BorderAppliesTo": "AllPages",
    "BorderDistanceFrom": "Text",
    "BottomMargin": 56.7,
    "DifferentFirstPageHeaderFooter": false,
    "FirstPageTray": 0,
    "FooterDistance": 42.5,
    "Gutter": 0.0,
    "HeaderDistance": 35.45,
    "LeftMargin": 56.7,
    "LineNumberCountBy": 0,
    "LineNumberDistanceFromText": 0.0,
    "LineNumberRestartMode": "RestartPage",
    "LineStartingNumber": 1,
    "Orientation": "Portrait",
    "OtherPagesTray": 0,
    "PageHeight": 841.9,
    "PageNumberStyle": "Arabic",
    "PageStartingNumber": 1,
    "PageWidth": 595.3,
    "PaperSize": "A4",
    "RestartPageNumbering": false,
    "RightMargin": 56.7,
    "RtlGutter": true,
    "SectionStart": "NewPage",
    "SuppressEndnotes": false,
    "TopMargin": 56.7,
    "VerticalAlignment": "Top",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pagesetup",
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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetSectionPageSetup.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetSectionPage.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetSectionPage.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetSectionPage.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetSectionPage.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetSectionPage.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetSectionPage.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetSectionPage.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetSectionPageSetup.go" >}}
{{< /tab >}}
{{< /tabs >}}