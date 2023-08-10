# Scroll Milestone

### 
When the user scrolls down the page.

This will only be added to specific pages to cut down on server calls.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "scroll",
    "scroll": {
        "eventName": "scroll_milestone",
        "mileStone": <mileStone>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|scroll.eventName|string|Static value|scroll\_milestone|
|scroll.mileStone|number|Milestone scrolled on the page (25, 50, 75, 100)|25, 50, 75, 100|




