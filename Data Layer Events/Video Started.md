# Video Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Video Started",
    "video": {
        "eventName": "video_start",
        "videoName": "<videoName>",
        "videoURL": "<videoURL>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example
| --- | --- | --- | --- |
|video.eventName|string|Static value, see examples|video\_start|
|video.videoName|string|Video Name|Meechie's Story|
|video.videoURL|string|URL of video|https://www.youtube.com/embed/lpprkE_2eNs?rel=0|




