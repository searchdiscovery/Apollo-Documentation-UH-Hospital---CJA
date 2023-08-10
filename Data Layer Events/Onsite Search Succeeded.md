# Onsite Search Succeeded

When the results of search appear on the screen

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Succeeded",
    "searchResults": {
        "contentType": "<contentType>",
        "eventName": "view_search_results",
        "resultCount": <resultCount>,
        "searchRefinements": "<searchRefinements>",
        "searchTerm": "<searchTerm>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|searchResults.contentType|string|When used with the "search" event, this attribute will distinguish between "Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education" and "Find a Location".|"Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education", "Find a Location"|
|searchResults.eventName|string|static value, see examples|view\_search\_results|
|searchResults.resultCount|number|The number of search results returned|2, 300, 1000|
|searchResults.searchRefinements|string|The refinements values the user added to filter search|"Insursance:Anthem\|Treats:adults,seniors"|
|searchResults.searchTerm|string|Term the user used in search|"cancer", "dr. smith"|




