# User Signed Out

### 
When the user successfully deauthenticates.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Signed Out",
    "user": {
        "event": "logout",
        "loginStatus": "<loginStatus>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|
| --- | --- | --- | --- |
|user.event|string|Static value|logout|
|user.loginStatus|string|Describes the login state of the user|logged in, logged out, guest|




