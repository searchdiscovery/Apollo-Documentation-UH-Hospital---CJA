# User Signed In

### 
When the user successfully authenticates.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Signed In",
    "user": {
        "event": "login",
        "loginStatus": "<loginStatus>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|user.event|string|Static value|login, logout|
|user.loginStatus|string|Describes the login state of the user|logged in, logged out, guest|




