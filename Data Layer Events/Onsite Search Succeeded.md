# Onsite Search Succeeded

When the results of search appear on the screen

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Succeeded",
    "searchResults": {
        "eventName": "view_search_results",
        "contentType": "<contentType>",
        "searchRefinements": [
            {
              "filter": "<filter>",
              "filter": "<filter>"
            }
        ],
        "searchTerm": "<searchTerm>",
        "resultCount": <resultCount>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|searchResults.eventName|string|static value, see examples|view\_search\_results|
|searchResults.contentType|string|When used with the "search" event, this attribute will distinguish between "Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education" and "Find a Location".|"Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education", "Find a Location"|
|searchResults.searchRefinements[n].filter|string|Describes the the filter types and filter detail applied on searches|<br>Insursance:Anthem</br><br>Treats:adults,seniors</br>|
|searchResults.searchTerm|string|Term the user used in search|"cancer", "dr. smith"|
|searchResults.resultCount|number|The number of search results returned|2, 300, 1000|



<p><img title="RFI Complete" src="https://github.com/searchdiscovery/Apollo-Documentation-UH-Hospital---CJA/blob/main/images/View%20Search%20Results.png?raw=true" alt="" /></p>
