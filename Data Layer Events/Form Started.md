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




