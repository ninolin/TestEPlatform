- [回首頁](../../ePlatformApiSepc.md) 

# Step1. 輸入身份證、生日

```json
POST /password/lock/identity
```

- Request Parameters
    
    Header
    
    ```json
    Content-Type: application/json
    ```
    
    Body
    
    ```json
    {
        "idno": "身份證字號",
        "birthday":"19840201",
        "code":"驗證碼",
        "uuid":"驗證碼uid"
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
            "token": "eyJhbGciOiJIUzI1NiJ9.eyJvd25lciI6IlgyMjA1MDk4MzYiLCJiZGF0ZSI6IjE5ODQtMDItMDEiLCJleHAiOjE2NjY3NzAwOTl9.nwyz9KKX24LbmQrQLKiyiVp-jA8fUZoRv9lkQlvVICo",
            "accountInfo": [
                {
                    "bussKind": 0,
                    "branch": "8151",
                    "account": "9806088",
                    "mobileNo": "09****8791",
                    "email": "r********g@tssco.com.tw"
                }
            ]
        }
    }
    ```