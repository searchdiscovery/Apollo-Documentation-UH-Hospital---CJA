# Download Link Clicked

User clicks downloadable links. These events will be automatically detected and fired for any `<a>` tag clicked by a user ad long as the existing data-eventName attribute is available on the <a> tag: 
  
  `data-eventName` 

The data attributes and events below are primarily here for cases in which a non anchor tag is used as a link. 
For example, if a `<button>` tag is used in combination with Javascript to represent a download link, you would need to add these attributes to manually fire the event.

## HTML Data Attributes

```html
<button
  data-eventName="file_download"
  data-fileName="<fileName>"
  data-fileType="<fileType>"
>
```


## Javascript Code
```js
// When:
// User clicks a non anchor tag used for an action, i.e. <button>

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

|Path|Type|Description|Example|
| --- | --- | --- | --- | 
|linkInfo.eventName|string|Static value, see examples|file\_download|
|linkInfo.fileName|string|Indicates the filename for download link tracking.|Year End 2012.pdf, Operating Instructions.doc`|
|linkInfo.fileType|string|Indicates the file type for download link tracking.|pdf, doc, csv, dmp, zip|
|linkInfo.linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|
|linkInfo.linkText|string|Text value of the anchor tag link|Click Here, Pay Now, Read More, Learn More|
|linkInfo.linkURL|string|This will include the href link value|https:\/\/www.uhhospitals.org\/patients-and-visitors\/billing-insurance-and-medical-records\/pay-my-bill|

<p><img title="" src="https://github.com/searchdiscovery/Apollo-Documentation-UH-Hospital---CJA/blob/main/images/Download%20Link.png?raw=true" alt="" /></p>

