```
GET/myPage
```
 - Request
 ```
 - header
 {
     loginUserId:
     Integer
 }
 ```
 - Response
 ```
 SUCCESS{"code:200",
 [{
    "eventId": 0,
    "haveDialog": true,
    "messageId": 0,
    "roomId": 0,
    "sendDateNow": "2019-11-21T07:40:39.544Z",
    "toUserId": "string",
    "type": 0
  }
]}
```
```
FAIL {"code" : 500, "message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}

```
PUT/myPage
```
 - Request
```
-header
{
    loginUserId:
    Integer
}
-body
{
  "admin": true,
  "classOf": 0,
  "iconIndex": 0,
  "id": "string",
  "myCalendarId": 0,
  "pw": "string"
}
```
 - Response
```
SUCCESS {"code" : 200, {
  "admin": true,
  "classOf": 0,
  "iconIndex": 0,
  "id": "string",
  "myCalendarId": 0,
  "pw": "string"
}}

```
```
FAIL {"code": 500, "message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"} 
```