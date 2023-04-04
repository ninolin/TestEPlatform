- [回首頁](../../ePlatformApiSepc.md) 

# Step3. 驗證OTP

```json
POST /password/lock/otp/verify
```

- Request Parameters
    
    Header
    
    ```json
    Content-Type: application/json
    Authorization: Bearer {jwt}
    ```
    
    Body
    
    ```json
    {
        "bussKind":0,
        "branch":"8151",
        "account":"9806088",
        "authKey": "u08AN0",
        "authSeq": "643719"
    }
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
        "response": "Success"
    }
    ```