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
{
    "index": Int,
    "subject": String,
    "teacher": String
}
```
- Response
```
SUCCESS {"code": 200, "message": "Success", "timetables":[{
    "index": Int,
    "subject": String
}]}
```
```
FAIL {"code": 500,"message":"FAIL"}
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
SUCCESS {"code": 200, "message": "Success", "timetables":[{
    "index": Int,
    "subject": String
}]}
```
```
FAIL {"code": 500,"message":"FAIL"}
```