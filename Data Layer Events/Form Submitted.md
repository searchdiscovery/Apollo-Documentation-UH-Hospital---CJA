# Form Submitted

### 
OUT OF SCOPE for initial project. If another form (non epic) needs submit tracking using this data layer event. 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Form Submitted",
    "form": {
        "eventName": "submit_appointment",
        "formType": "<formType>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|form.eventName|string|Static value, see examples|submit\_appointment|
|form.formType|string|Form type used for grouping of similar forms in reports.  |Address, Contact, Comment, Review, Payment|




