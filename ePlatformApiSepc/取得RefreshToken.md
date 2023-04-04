- [回首頁](../ePlatformApiSepc.md)

# 取得refresh token

```json
POST /auth/refreshToken
```

- Request Parameters
    
    Header
    
    ```json
    Content-Type: application/json
    Authorization: Bearer {jwt}
    ```
    
    Body
    
    ```json
    {}
    ```
    

- Responses
    
    Header
    
    ```json
    Content-Type: application/json
    Authorization: Bearer {jwt}
    ```
    
    Body
    
    ```json
    {
        "status": true,
        "code": "00000",
        "stringCode": "success",
        "message": "成功",
        "response": "eyJhbGciOiJIUzI1NiJ9.eyJvd25lciI6IlgyMjA1MDk4MzYiLCJYMjIwNTA5ODM2IjoiW01fU18wMDFfOTgwNjA4OF0iLCJleHAiOjE2NjM2MzY1ODJ9.i4GwKQM06X_UQuQWLzKSQ2utCckQ_3oVibTRAdrHheA"
    }
    ```