# Page Load Completed
This event fires upon page completion and after page load started.
## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  'event': 'Page Load Completed',
  'eventName': 'page_view'
});
```
