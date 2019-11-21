```
GET/message
```
 - Request
 ```
 - header 
 {
     loginUserId:
     Integer
 }

```
  - Respones
```
SUCCESS {"code: 200,
"message": "Success",
[
  {
    "eventId": 0,
    "haveDialog": true,
    "messageId": 0,
    "roomId": 0,
    "sendDateNow": "2019-11-21T06:38:51.247Z",
    "toUserId": "string",
    "type": 0
  }
]}
```
```
FAIL {"code" : 500, "message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
```

```
POST/message/{messageId}
```
 - Request
```
 - header
 {
     loginUserId:
     Integer
 }
 - body
 {
  "status": true
 }
 ```
 - Response
 ```
 SUCCESS {"code":200,"message":"Ok", "string"}
 ```
 ```
 FAIL {"code":500,"message":"FAIL"}
 FAIL {"code": 403,"message": "Forbidden"}
 ```

 ```
 DELETE/message/
 {messageId}
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
  SUCCESS {"code":
  200, "message":
  "Ok",
  [{
    "eventId": 0,
    "haveDialog": true,
    "messageId": 0,
    "roomId": 0,
    "sendDateNow": "2019-11-21T07:03:49.495Z",
    "toUserId": "string",
    "type": 0
  }]}
  ```
  ```
  FAIL {"code": 500,"message" : "FAIL"}
  FAIL {"code": 403,"message":"Forbidden"}
  ```






 
