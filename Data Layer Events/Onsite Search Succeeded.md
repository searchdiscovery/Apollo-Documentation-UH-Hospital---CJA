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
        "searchRefinements": [{
            "location": "<filter>",
            "insurance": "<filter>",
            "appointmentDate": "<filter>",
            "language": "<filter>",
            "providerGender": "<filter>",
            "treats": "<filter>",
            "newPatients": "<filter>",
            "onlineScheduling": "<filter>",
            "requestAnAppointment":"<filter>"
        }],
        "searchTerm": "<searchTerm>",
        "resultCount": < resultCount >
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|searchResults.eventName|string|static value, see examples|view\_search\_results|
|searchResults.contentType|string|When used with the "search" event, this attribute will distinguish between "Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education" and "Find a Location".|"Site Search", "Treatments & Conditions", "Diagnostics", "Find a Doctor", "Prescription Drugs", "Clinical Trials", "Medical Education", "Find a Location"|
|searchResults.searchRefinements[n].location|string|String containing the zip code|location:44101|
|searchResults.searchRefinements[n].insurance|string|String containing the selected insurance dropdown value|insursance:Anthem|
|searchResults.searchRefinements[n].appointmentDate|string|String containing the appointment date|appointmentDate:12-2-2023|
|searchResults.searchRefinements[n].language|string|String containing the selected dropdown value|language:spanish|
|searchResults.searchRefinements[n].providerGender|string| String containing the selected filters |providerGender:Female|
|searchResults.searchRefinements[n].treats|string|String containing the selected filters |treats:adults,seniors|
|searchResults.searchRefinements[n].newPatients|string|set to undefined if not selected|newPatients:yes|
|searchResults.searchRefinements[n].onlineScheduling|string|set to undefined if not selected |onlineScheduling:yes|
|searchResults.searchRefinements[n].requestAnAppointment|string|set to undefined if not selected |requestAnAppointment:yes|
|searchResults.searchTerm|string|Term the user used in search|"cancer", "dr. smith"|
|searchResults.resultCount|number|The number of search results returned|2, 300, 1000|



<p><img title="RFI Complete" src="https://github.com/searchdiscovery/Apollo-Documentation-UH-Hospital---CJA/blob/main/images/View%20Search%20Results.png?raw=true" alt="" /></p>
