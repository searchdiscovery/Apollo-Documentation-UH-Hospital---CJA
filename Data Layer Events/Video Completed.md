# Video Completed

### 
When the user completes a video.


## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Video Completed",
    "video": {
        "eventName": "video_complete",
        "videoName": "<videoName>",
        "videoURL": "<videoURL>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|video.eventName|string|Static value|video\_complete|
|video.videoName|string|Video Name|Meechie's Story|
|video.videoURL|string|URL of video|https://www.youtube.com/embed/lpprkE_2eNs?rel=0|




