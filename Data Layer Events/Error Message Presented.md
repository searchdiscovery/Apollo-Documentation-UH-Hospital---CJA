# Error Message Presented

### 
When a user receives an error not related to a form (such as "page not found")


## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Error Message Presented",
    "error": {
        "errorMessage": "<errorMessage>",
        "errorType": "<errorType>",
        "eventName": "page_error"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- | 
|error.errorMessage|string|Used with the "error" and "form_error" events to describe the error that was encountered.|404, page under construction|
|error.errorType|string|General type of error presented|Payment, System, Form|
|error.eventName|string|Static value, see examples|"page\_error"|



## Form Error
<p><img title="RFI Complete" src="https://github.com/searchdiscovery/Apollo-Documentation-UH-Hospital---CJA/blob/main/images/Form%20Error.png?raw=true" alt="" /></p>

## Page Error
<p><img title="RFI Complete" src="https://github.com/searchdiscovery/Apollo-Documentation-UH-Hospital---CJA/blob/main/images/Page%20Error.png?raw=true" alt="" /></p>
