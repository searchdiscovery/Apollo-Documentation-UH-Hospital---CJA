# Error Message Presented

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Error Message Presented",
    "error": {
        "errorMessage": "<errorMessage>",
        "errorType": "<errorType>",
        "eventName": "<eventName>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|error.errorMessage|string|test of the error||||||||
|error.errorType|string|General type of error presented|Payment, System, Form|||||||
|error.eventName|string|Static value, see examples|"form\_error", "page\_error"|||||||




