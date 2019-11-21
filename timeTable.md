시간표 수정
-
```
PUT/timetable
```
 - Request
```
- header
{
    loginUserId: Integer
}
- body
[{
    "subject": "string",
    "teacher": "string",
    "timeTableIndex": 0
}]
```
- Response
```
SUCCESS {"code": 200, [{
    "subject": "string",
    "teacher": "string",
    "timeTableIndex": Integer
  }]
}
```
```
FAIL {"code": 500,"message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
```
시간표 전체 보기
-
```
GET/timetable/
```
 - Request
```
{

}
```
- Response
```
SUCCESS {"code": 200, [{
    "subject": "string",
    "teacher": "string",
    "timeTableIndex": Integer
  }]
}
```
```
FAIL {"code": 500,"message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
```