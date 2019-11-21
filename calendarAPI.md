일정 추가
-
```
POST/schedule/{calendarId}
```
 - Request
```
- header
{
    loginUserId: Integer
}
- body
{
    scheduleContent: String,
    scheduleTitle: String,
    startDate: String,
    endDate: String
}
```
- Response
```
SUCCESS {"code": 200, "message": "Success", [{
    scheduleContent: String,
    scheduleTitle: String,
    startDate: String,
    endDate: String
}]}
```
```
FAIL {"code": 500,"message":"FAIL"}
```
일정 수정
-
```
PUT/calendar/{scheduleId}
```
 - Request
```
- header
{
    loginUserId: Integer
}
- body
{
    scheduleContent: String,
    scheduleTitle: String,
    startDate: String,
    endDate: String
}
```
- Response
```
SUCCESS {"code": 200, "message": "Success", [{
    scheduleContent: String,
    scheduleTitle: String,
    startDate: String,
    endDate: String
}]}
```
```
FAIL {"code": 500,"message":"FAIL"}
```
내 일정 보기
-
```
GET/myCalendar
```
 - Request
```
- header
{
    loginUserId: Integer
}
```
- Response
```
SUCCESS {"code": 200, "message": "Success", [{
    scheduleContent: String,
    scheduleTitle: String,
    startDate: String,
    endDate: String
}]}
```
```
FAIL {"code": 500,"message":"FAIL"}
```
일정 상세보기
-
```
GET/calendar/{scheduleId}
```
 - Request
```
- header
{
    loginUserId: Integer
}
```
- Response
```
SUCCESS {"code": 200, "message": "Success", [{
    scheduleContent: String,
    scheduleTitle: String,
    startDate: String,
    endDate: String
}]}
```
```
FAIL {"code": 500,"message":"FAIL"}
```
일정 삭제
-
```
DELETE/calendar/{scheduleId}
```
 - Request
```
- header
{
    loginUserId: Integer
}
```
- Response
```
SUCCESS {"code": 200, "message": "Ok"}
```
```
FAIL {"code": 500,"message":"FAIL"}
```