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
SUCCESS {"code": 200, [{
  "calendarId": 0,
  "endDate": "string",
  "scheduleContent": "string",
  "scheduleId": 0,
  "scheduleTitle": "string",
  "startDate": "string"
}}
```
```
FAIL {"code": 500,"message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
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
SUCCESS {"code": 200, "message": "Success"}
```
```
FAIL {"code": 500,"message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
```
내 일정 모두 보기
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
SUCCESS {"code": 200, [{
    "calendarId": 0,
    "endDate": "string",
    "scheduleContent": "string",
    "scheduleId": 0,
    "scheduleTitle": "string",
    "startDate": "string"
  }]
}
```
```
FAIL {"code": 500,"message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
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
SUCCESS {"code": 200,  {
  "calendarId": Integer,
  "endDate": "string",
  "scheduleContent": "string",
  "scheduleId": Integer,
  "scheduleTitle": "string",
  "startDate": "string"
}}
```
```
FAIL {"code": 500,"message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
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
FAIL {"code": 403,"message": "Forbidden"}
```
학교 일정 보기
-
```
GET/schoolCalendar
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
SUCCESS {"code": 200, "message": "scheduleList": [{
      "calendarId": Integer,
      "endDate": "string",
      "scheduleContent": "string",
      "scheduleId": Integer,
      "scheduleTitle": "string",
      "startDate": "string"
    }],
  "schoolCalendarId": Integer"}
```
```
FAIL {"code": 500,"message":"FAIL"}
FAIL {"code": 403,"message": "Forbidden"}
```