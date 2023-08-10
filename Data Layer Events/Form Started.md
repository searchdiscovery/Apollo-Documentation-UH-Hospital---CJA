# Form Started

### 
Begin the `Schedule Me Now` flow

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Form Started",
    "form": {
        "eventName": "begin_openScheduling",
        "formType": "<formType>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|form.eventName|string|Static value, see examples|begin\_openScheduling, submit\_appointment|
|form.formType|string|Form type used for grouping of similar forms in reports.  |Address, Contact, Comment, Review, Payment|



<p><img title="RFI Complete" src="https://github.com/searchdiscovery/Apollo-Documentation-UH-Hospital---CJA/blob/main/images/Schedule%20Me%20Now.png?raw=true" alt="" /></p>
