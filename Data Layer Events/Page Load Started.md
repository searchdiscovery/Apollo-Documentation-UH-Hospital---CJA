# Page Load Started

### Page Load Started is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the first event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
    "page": {
        "blogPostCategory": "<blogPostCategory>",
        "blogPostTags": "<blogPostTags>",
        "facilityTypeID": "<facilityTypeID>",
        "pageCategory": "<pageCategory>",
        "physicalLocationID": "<physicalLocationID>",
        "physicalLocationName": "<physicalLocationName>",
        "serviceLine": "<serviceLine>"
    },
    "webCampaigns": {
        "campaign": "<campaign>",
        "medium": "<medium>",
        "source": "<source>"
    },
    "webPageDetails": {
        "webReferrer": "<webReferrer>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page.blogPostCategory|string|Applies to the blog only, and displays the category of the post being viewed.|blog, patient stories, podcast|||||||
|page.blogPostTags|string|A comma separated list of tags that describe the blog post being viewed.|Bariatric Surgery, Digestive Health, Weight Loss Surgery|||||||
|page.facilityTypeID|string|When viewing a location page, this parameter provides a comma separated list of IDs that describe the type of facility being viewed.||||||||
|page.pageCategory|string|\[set globally across all events\] Used for grouping pages \(or screens\) into high level categories.  Examples: Blog, Find a Doctor, Locations, Services, Scheduling, etc|Blog, Find a Doctor, Locations, Services, Scheduling, etc|||||||
|page.physicalLocationID|string|When viewing content related to a physical location, this paremeter provides an ID of the facility.||||||||
|page.physicalLocationName|string|When viewing content related to a physical location, this parameter provides a name of the facility.||||||||
|page.serviceLine|string|\[set globally across all events\] Identifies the service line that this page most accurately supports.  Example: "CIHM", "Dermatology".  Default value should be "none".  On the blog the "topic" is equal to a service line.||||||||
|webCampaigns.campaign|string|utm campaign||||||||
|webCampaigns.medium|string|utm medium||||||||
|webCampaigns.source|string|utm source||||||||
|webPageDetails.webReferrer|string|webPageDetails.webReferrer||||||||




