- [回首頁](../../ePlatformApiSepc.md) 

# Step2. 產生OTP

```json
POST /password/lock/otp/gen
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
        "account":"9806088"
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
        "response": {
            "authSeq": "023193",
            "token": null (先不看 等之後我再看需不需要)
        }
    }
    ```