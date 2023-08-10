# Video Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Video Started",
    "video": {
        "eventName": "<eventName>",
        "videoName": "<videoName>",
        "videoURL": "<videoURL>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|video.eventName|string|Static value, see examples|video\_start, video\_complete|||||||
|video.videoName|string|Video Name|Twitch\_FPS, Age of Empires, Halo|||||||
|video.videoURL|string|url of video||||||||




