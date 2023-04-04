- [回首頁](../../ePlatformApiSepc.md) 

# 驗證OTP驗證碼

[http://172.24.42.56/eservice/pushapi](http://172.24.42.56/eservice/pushapi)

```json
POST /otp/gen
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
        "header": {
            "version": "0.0.1",
            "origin": "TG",
            "bussKind": 0,
            "branch": "1111",
            "account": "12345678",
            "registerId": "A000000000"
        },
        "body": {
            "otpId": "pwdUnlock",
            "authKey": "tA1O96",
            "authSeq": "127829"
        }
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
        "status": {
            "status": true,
            "code": "00000",
            "stringCode": "success",
            "message": "成功",
            "messageEN": "Success!"
        },
        "dateList": "Success"
    }
    ```