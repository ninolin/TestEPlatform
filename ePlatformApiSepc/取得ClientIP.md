- [回首頁](../ePlatformApiSepc.md) 

# 取得Client IP

```json
GET /client/ip
```

- Request Parameters
    
    Header
    
    ```json
    Content-Type: application/json
    Authorization: Bearer {jwt}
    ```
    
    Body
    
    ```json
    none
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
            "clientIp": "172.24.20.87"
        }
    }
    ```