# Download Link Clicked

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Download Link Clicked",
    "linkInfo": {
        "eventName": "<eventName>",
        "fileName": "<fileName>",
        "fileType": "<fileType>",
        "linkId": "<linkId>",
        "linkText": "<linkText>",
        "linkURL": "<linkURL>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkInfo.eventName|string|Static value, see examples|link\_click, link\_click|||||||
|linkInfo.fileName|string|Indicates the filename for download link tracking.|Year End 2012.pdf, Operating Instructions.doc`|||||||
|linkInfo.fileType|string|Indicates the file type for download link tracking.|pdf, doc, csv, dmp, zip|||||||
|linkInfo.linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|||||||
|linkInfo.linkText|string|Text value of the anchor tag link|Click Here, Pay Now, Read More, Learn More|||||||
|linkInfo.linkURL|string|This will include the href link value|https:\/\/www.uhhospitals.org\/patients-and-visitors\/billing-insurance-and-medical-records\/pay-my-bill|||||||




