# CTA Link Clicked

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "CTA Link Clicked",
    "linkInfo": {
        "eventName": "<eventName>",
        "linkClass": "<linkClass>",
        "linkId": "<linkId>",
        "linkOutbound": <linkOutbound>,
        "linkText": "<linkText>",
        "linkURL": "<linkURL>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkInfo.eventName|string|Static value, see examples|link\_click, link\_click|||||||
|linkInfo.linkClass|string|CSS class value,  if applicable to the link||||||||
|linkInfo.linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|||||||
|linkInfo.linkOutbound|boolean|If the link is directing to a different domain|true, false|||||||
|linkInfo.linkText|string|Text value of the anchor tag link|Click Here, Pay Now, Read More, Learn More|||||||
|linkInfo.linkURL|string|This will include the href link value|https:\/\/www.uhhospitals.org\/patients-and-visitors\/billing-insurance-and-medical-records\/pay-my-bill|||||||




