# Trust login

```json
POST /auth/login?trustKey={token}&origin={origin}
```

- Request Parameters
    
    Header
    
    ```json
    Content-Type: application/json
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
    
    accountData欄位說明：
    
    | 欄位 | 說明 |
    | --- | --- |
    | bhName | 證券分公司名稱 |
    | bhno | 證券分行代碼 |
    | fbhName | 期貨分公司名稱 |
    | fbhno | 期貨分行代碼 |
    | accountType | S=證券 F=期貨 U=複委託 |
    | agType | M=本人帳號, D=代操帳號 |
    
    ```json
    {
        "status": true,
        "code": "00000",
        "stringCode": "success",
        "message": "成功",
        "response": {
            "token": "eyJhbGciOiJIUzI1NiJ9.eyJvd25lciI6IlExMDI5Mzc2OTMgIiwiYWdlbnQiOlsiUTEwMjkzNzY5MyIsIjE2Nzk1ODU2IiwiUzIyMDQ3OTY4OSJdLCJmaXJzdExvZ2luIjoiTiIsIlExMDI5Mzc2OTMiOlsiS2tseGVKeXl3R0pST203Y0plWWFINkdVL1JWU1diSFlTMTFQMUhHQ1VrTT0iLCJrQ3FGNk9GbENYMXRDdG5DTWNJSlNiUnRhUTVJaFBlYWduOXN2SEhtbktRPSIsImlUMGZQZUhxYU1iMWdDeHJTdkVoeERuR1NrZWJBYkFwRTllZHBDMTJ4VWs9Il0sIjE2Nzk1ODU2IjpbIjNWUHR0TElMcTZHMUIxeDV1NGhMbFpoU2JrRSt6Wk01MHVjRUJhRlUwUmc9IiwidEUzZ25saWt2OEdxbE5RdjR3ZXExaUx2aXFQMkhIY2lnMEZlSFpsSmFhbz0iLCI5cklxWlAwSnhhclBIblpKQjdSZXJ1THFkdDJMMnFJZnpZellXQ0lKWmlrPSJdLCJTMjIwNDc5Njg5IjpbIkVkKzJGNWwvaGtGRWNrYy91dDhVWGd4N25hZjRPRCtHN0VXTldEQ0xBSlU9Il0sImV4cCI6MTY3OTAzNDk2N30.xB13FforxtVsCGFf3csIN_u0_OtezI8XI0ckiUjazzQ",
            "clientIp": "172.24.20.87",
            "cert": "",
            "userInfo": {
                "custName": "吳＊＊＊＊",
                "idNumber": "Q102937693",
                "count": "7",
                "pwNotice": "N",
                "firstLogin": "N",
                "accountData": [
                    {
                        "bhName": "台北營業部",
                        "bhno": "8150",
                        "fbhName": "台北總公司",
                        "fbhno": "8150",
                        "account": "6741668",
                        "idno": "Q102937693",
                        "eFlag": "Y",
                        "accountType": "S",
                        "sFlag": "N",
                        "subAccount": "",
                        "agType": "M",
                        "agName": "",
                        "agNo": "999",
                        "agHide": "N",
                        "iFlag": "N",
                        "fFlag": "",
                        "apiFlag": "N",
                        "natural": "Y",
                        "sex": null,
                        "birthDate": null,
                        "cert": ""
                    },
                    {
                        "bhName": "建北分公司",
                        "bhno": "8151",
                        "fbhName": "建北分公司",
                        "fbhno": "8151",
                        "account": "0026676",
                        "idno": "Q102937693",
                        "eFlag": "Y",
                        "accountType": "S",
                        "sFlag": "X",
                        "subAccount": "",
                        "agType": "M",
                        "agName": "",
                        "agNo": "999",
                        "agHide": "N",
                        "iFlag": "N",
                        "fFlag": "",
                        "apiFlag": "N",
                        "natural": "Y",
                        "sex": null,
                        "birthDate": null,
                        "cert": ""
                    },
                    {
                        "bhName": "建北分公司",
                        "bhno": "8151",
                        "fbhName": "建北分公司",
                        "fbhno": "8151",
                        "account": "0133705",
                        "idno": "16795856",
                        "eFlag": "Y",
                        "accountType": "S",
                        "sFlag": "N",
                        "subAccount": "",
                        "agType": "D",
                        "agName": "買代測試１",
                        "agNo": "999",
                        "agHide": "N",
                        "iFlag": "Y",
                        "fFlag": "",
                        "apiFlag": "Y",
                        "natural": "",
                        "sex": null,
                        "birthDate": null,
                        "cert": "[\"-1\",\"6072AAB8\",\"31\",\"2023-03-07 16:09:17.0\",\"Windows 10/Chrome 110.0.0.0\"], [\"-1\",\"6E7FC0DBE14FE6781C7257B817DEF2D7\",\"31\",\"2023-03-15 13:53:44.697\",\"x86_64/16.0\"], [\"-1\",\"44E1BB86E5D8E72DD1FB6D826EEB6EC2\",\"31\",\"2023-03-15 14:19:52.777\",\"x86_64/16.2\"], [\"-1\",\"6072BED5\",\"31\",\"2023-03-15 14:21:48.0\",\"iPhone12,8/16.1.1\"], [\"-1\",\"4385C61A0D7C0C13EDA87D8610E31D10\",\"31\",\"2023-03-15 14:24:17.973\",\"HTC U12 life\"], [\"-1\",\"6072BF76\",\"31\",\"2023-03-15 16:38:23.0\",\"Android SDK built for x86\"], [\"-1\",\"6072BFC8\",\"31\",\"2023-03-15 18:07:08.0\",\"iPhone14,2/15.4.1\"], [\"-1\",\"38C27AC1024E10838015B8EB141C4AB2\",\"31\",\"2023-03-15 18:38:34.36\",\"SM-G955U\"], [\"-1\",\"6072C177\",\"31\",\"2023-03-16 09:49:49.0\",\"sdk_gphone_x86\"], [\"-1\",\"31BD413E4C38A807E7463079CB42C08A\",\"31\",\"2023-03-16 11:36:04.997\",\"iPhone14,5/16.0\"], [\"-1\",\"570B1CF2F1C6EF456616B51B884F86AD\",\"31\",\"2023-03-17 11:50:45.333\",\"iPhone14,2/15.4.1\"]"
                    },
                    {
                        "bhName": "高雄分公司",
                        "bhno": "815A",
                        "fbhName": "高雄分公司",
                        "fbhno": "815A",
                        "account": "7777932",
                        "idno": "16795856",
                        "eFlag": "Y",
                        "accountType": "S",
                        "sFlag": "X",
                        "subAccount": "",
                        "agType": "D",
                        "agName": "買代測試１",
                        "agNo": "999",
                        "agHide": "N",
                        "iFlag": "N",
                        "fFlag": "",
                        "apiFlag": "N",
                        "natural": "",
                        "sex": null,
                        "birthDate": null,
                        "cert": "[\"-1\",\"6072AAB8\",\"31\",\"2023-03-07 16:09:17.0\",\"Windows 10/Chrome 110.0.0.0\"], [\"-1\",\"6E7FC0DBE14FE6781C7257B817DEF2D7\",\"31\",\"2023-03-15 13:53:44.697\",\"x86_64/16.0\"], [\"-1\",\"44E1BB86E5D8E72DD1FB6D826EEB6EC2\",\"31\",\"2023-03-15 14:19:52.777\",\"x86_64/16.2\"], [\"-1\",\"6072BED5\",\"31\",\"2023-03-15 14:21:48.0\",\"iPhone12,8/16.1.1\"], [\"-1\",\"4385C61A0D7C0C13EDA87D8610E31D10\",\"31\",\"2023-03-15 14:24:17.973\",\"HTC U12 life\"], [\"-1\",\"6072BF76\",\"31\",\"2023-03-15 16:38:23.0\",\"Android SDK built for x86\"], [\"-1\",\"6072BFC8\",\"31\",\"2023-03-15 18:07:08.0\",\"iPhone14,2/15.4.1\"], [\"-1\",\"38C27AC1024E10838015B8EB141C4AB2\",\"31\",\"2023-03-15 18:38:34.36\",\"SM-G955U\"], [\"-1\",\"6072C177\",\"31\",\"2023-03-16 09:49:49.0\",\"sdk_gphone_x86\"], [\"-1\",\"31BD413E4C38A807E7463079CB42C08A\",\"31\",\"2023-03-16 11:36:04.997\",\"iPhone14,5/16.0\"], [\"-1\",\"570B1CF2F1C6EF456616B51B884F86AD\",\"31\",\"2023-03-17 11:50:45.333\",\"iPhone14,2/15.4.1\"]"
                    },
                    {
                        "bhName": "建北分公司",
                        "bhno": "8151",
                        "fbhName": "建北分公司",
                        "fbhno": "8151",
                        "account": "0027866",
                        "idno": "S220479689",
                        "eFlag": "Y",
                        "accountType": "S",
                        "sFlag": "X",
                        "subAccount": "",
                        "agType": "D",
                        "agName": "買代測試１",
                        "agNo": "999",
                        "agHide": "N",
                        "iFlag": "N",
                        "fFlag": "",
                        "apiFlag": "N",
                        "natural": "",
                        "sex": null,
                        "birthDate": null,
                        "cert": "[\"-1\",\"6072AADD\",\"31\",\"2023-03-07 16:52:32.0\",\"x86_64/16.2\"], [\"-1\",\"6072ADC3\",\"31\",\"2023-03-08 16:15:28.0\",\"iPhone12,8/16.1.1\"], [\"-1\",\"6072B13D\",\"31\",\"2023-03-09 16:19:43.0\",\"Windows 10/Chrome 110.0.0.0\"], [\"-1\",\"1734A8553752A6DA784AB03A679AE1E4\",\"31\",\"2023-03-15 10:38:47.453\",\"iPhone12,1/15.6.1\"], [\"-1\",\"770166174B4B93B47E73B94033B22E0D\",\"31\",\"2023-03-15 15:21:13.74\",\"x86_64/16.0\"]"
                    },
                    {
                        "bhName": "建北分公司",
                        "bhno": "8151",
                        "fbhName": "建北分公司",
                        "fbhno": "8151",
                        "account": "0026676",
                        "idno": "Q102937693",
                        "eFlag": "Y",
                        "accountType": "F",
                        "sFlag": "",
                        "subAccount": "",
                        "agType": "M",
                        "agName": "",
                        "agNo": "999",
                        "agHide": "N",
                        "iFlag": "N",
                        "fFlag": "N",
                        "apiFlag": "N",
                        "natural": "Y",
                        "sex": null,
                        "birthDate": null,
                        "cert": ""
                    },
                    {
                        "bhName": "建北分公司",
                        "bhno": "8151",
                        "fbhName": "建北分公司",
                        "fbhno": "8151",
                        "account": "0133705",
                        "idno": "16795856",
                        "eFlag": "Y",
                        "accountType": "F",
                        "sFlag": "",
                        "subAccount": "",
                        "agType": "D",
                        "agName": "吳＊源",
                        "agNo": "999",
                        "agHide": "N",
                        "iFlag": "Y",
                        "fFlag": "N",
                        "apiFlag": "N",
                        "natural": "",
                        "sex": null,
                        "birthDate": null,
                        "cert": "[\"-1\",\"6072AAB8\",\"31\",\"2023-03-07 16:09:17.0\",\"Windows 10/Chrome 110.0.0.0\"], [\"-1\",\"6E7FC0DBE14FE6781C7257B817DEF2D7\",\"31\",\"2023-03-15 13:53:44.697\",\"x86_64/16.0\"], [\"-1\",\"44E1BB86E5D8E72DD1FB6D826EEB6EC2\",\"31\",\"2023-03-15 14:19:52.777\",\"x86_64/16.2\"], [\"-1\",\"6072BED5\",\"31\",\"2023-03-15 14:21:48.0\",\"iPhone12,8/16.1.1\"], [\"-1\",\"4385C61A0D7C0C13EDA87D8610E31D10\",\"31\",\"2023-03-15 14:24:17.973\",\"HTC U12 life\"], [\"-1\",\"6072BF76\",\"31\",\"2023-03-15 16:38:23.0\",\"Android SDK built for x86\"], [\"-1\",\"6072BFC8\",\"31\",\"2023-03-15 18:07:08.0\",\"iPhone14,2/15.4.1\"], [\"-1\",\"38C27AC1024E10838015B8EB141C4AB2\",\"31\",\"2023-03-15 18:38:34.36\",\"SM-G955U\"], [\"-1\",\"6072C177\",\"31\",\"2023-03-16 09:49:49.0\",\"sdk_gphone_x86\"], [\"-1\",\"31BD413E4C38A807E7463079CB42C08A\",\"31\",\"2023-03-16 11:36:04.997\",\"iPhone14,5/16.0\"], [\"-1\",\"570B1CF2F1C6EF456616B51B884F86AD\",\"31\",\"2023-03-17 11:50:45.333\",\"iPhone14,2/15.4.1\"]"
                    }
                ]
            }
        }
    }
    ```