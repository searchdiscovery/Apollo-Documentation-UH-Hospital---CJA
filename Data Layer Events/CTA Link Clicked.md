# CTA Link Clicked

User clicks main CTA request info link. These events will be automatically detected and fired for any `<a>` tag clicked by a user ad long as the existing data-eventName attribute is available on the <a> tag: 
  
  `data-eventName` 

The data attributes and events below are primarily here for cases in which a non anchor tag is used as a link. 
For example, if a `<button>` tag is used in combination with Javascript to represent a download link, you would need to add these attributes to manually fire the event.

## HTML Data Attributes

```html
<button
  data-eventName="link_click"
  data-linkOutbound="<outbound>"
>
```


## Javascript Code
```js
// When:
// User clicks a non anchor tag used for an action, i.e. <button>

window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "CTA Link Clicked",
    "linkInfo": {
        "eventName": "<eventName>",
        "linkClass": "<linkClass>",
        "linkId": "<linkId>",
        "linkOutbound": "<linkOutbound>",
        "linkText": "<linkText>",
        "linkURL": "<linkURL>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkInfo.eventName|string|Static value, see examples|link\_click|||||||
|linkInfo.linkClass|string|CSS class value,  if applicable to the link||||||||
|linkInfo.linkId|string|Identifier of the link clicked||||||||
|linkInfo.linkOutbound|boolean|If the link is directing to a different domain|true, false|||||||
|linkInfo.linkText|string|Text value of the anchor tag link|Click Here, Pay Now, Read More, Learn More|||||||
|linkInfo.linkURL|string|This will include the href link value|https:\/\/www.uhhospitals.org\/patients-and-visitors\/billing-insurance-and-medical-records\/pay-my-bill|||||||




