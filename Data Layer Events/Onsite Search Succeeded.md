# Onsite Search Succeeded

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Succeeded",
    "searchResults": {
        "contentType": "<contentType>",
        "eventName": "<eventName>",
        "resultCount": <resultCount>,
        "searchRefinements": "<searchRefinements>",
        "searchTerm": "<searchTerm>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|searchResults.contentType|string|When used with the "search" event, this attribute will distinguish between "Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education" and "Find a Location".|"Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education", "Find a Location"|||||||
|searchResults.eventName|string|static value, see examples|view\_search\_results, search|||||||
|searchResults.resultCount|number|The number of search results returned||||||||
|searchResults.searchRefinements|string|The refinements values the user added to filter search||||||||
|searchResults.searchTerm|string|Term the user used in search||||||||




