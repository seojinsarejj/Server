회원
=
회원가입
-
```
POST/join
```
- STUDENT
    - Request
    ```
    {
        id: String,
        pw: String,
        classOf: Int
    }
    ```
    - Response
    ```
    SUCCESS {"code": 200, message: "Success"}
    ```
    ```
    FAIL {"code": 500, message:"FAIL"}
    
    ```
로그인
-
```
POST/login
```
 - Request
```
{
    id: String,
    pw: String,
}
```
- Response
```
SUCCESS {"code": 200, {
     classOf: Int,
     iconIndex: Int,
     id: String,
     loginUserId: Integer,
     myCalendarId: Integer
    }}
```
```
FAIL {"code": 500, message:"FAIL"}
FAIL {"code": 404, message:"Not found"}
```
로그아웃
-
```
POST/logout
```
 - Request
```
{
   
}
```
- Response
```
SUCCESS {"code": 200, message: "string"}
```
```
FAIL {"code": 500, message:"FAIL"}
FAIL {"code": 404, message:"Not found"}
```