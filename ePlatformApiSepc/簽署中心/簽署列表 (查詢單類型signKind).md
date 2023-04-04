- [回首頁](../../ePlatformApiSepc.md) 

# 簽署列表 (查詢單類型signKind)

```json
POST /sign/main/:singKind
```

singKind :

1.線上簽署 2.基本資料變更 3.線上測試 4.約定事項

- Request Parameters
    
    Header
    
    ```json
    Content-Type: application/json
    Authorization: Bearer {jwt}
    ```
    
    Body
    
    ```json
    {
        "bussKind": "業務別", 
        "origin" :"TG", //來源別
        "commCate": 0, //商品分類 0=ID歸戶 1=證券 2=期貨 3=複委託 4=衍生
        "idno": "身分證字號",
        "branch": "分號代碼",
        "account": "帳號",
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
        "response": [
            {
                "singKind": 1,
                "signId": "RY308_033",
                "itemName": "投資日本公司來臺上櫃(市)及興櫃股票之特別注意事項",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "033",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_037",
                "itemName": "證券商辦理應付當日沖銷券差有價證券借貸契約書（證券商與投資人）",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "037",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_042",
                "itemName": "黃金現貨風險預告書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "042",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_043",
                "itemName": "外國企業來台上市(櫃)有價證券風險預告書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "043",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_055",
                "itemName": "指數股票型高收益債券基金受益憑證買賣風險預告書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "055",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": " ",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_056",
                "itemName": "信用交易帳戶電子式追繳通知申請同意書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "056",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "1.已開立信用交易帳戶。\r\n2. 基本資料有留存電子郵件帳號。",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_088",
                "itemName": "買賣轉換公司債及交換公司債風險預告書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "088",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_089",
                "itemName": "指數投資證券買賣及申購賣回風險預告書(ETN",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "089",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_0C5",
                "itemName": "有價證券當日沖銷交易風險預告書暨概括授權同意書及證券商辦理應付當日沖銷券差有價證券借貸契約書（證券商與投資人）",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "0C5",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "1.須開戶滿三個月\r\n2.近一年內有十筆交易",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_138",
                "itemName": "指數股票型基金受益憑證買賣及申購買回風險預告書 (ETF)",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "138",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_153",
                "itemName": "指數股票型基金受益憑證買賣及申購買回風險預告書(槓桿反向型ETF)",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "153",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "具備下列條件之一：\r\n1.已開立信用交易帳戶。\r\n2.開戶滿三個月，近一年內買賣之認購（售）權證成交達十筆（含）以上。\r\n3.開戶滿三個月，近一年內買賣期貨、選擇權成交達十筆（含）以上",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_190",
                "itemName": "指數投資證券買賣及申購賣回風險預告書(槓桿反向期權策略型)(ETN)",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "190",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "具備下列條件之一：\r\n1.已開立信用交易帳戶。\r\n2.開戶滿三個月，近一年內買賣之認購（售）權證成交達十筆（含）以上。\r\n4.開戶滿三個月，近一年內買賣期貨、選擇權成交達十筆（含）以上",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_811",
                "itemName": "網路下單IP位址與他人相同聲明書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "811",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_813",
                "itemName": "買賣變更交易方法或受處置有價證券自動扣款同意書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "813",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "台新銀行交割戶專用",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_817",
                "itemName": "預約買零股同意書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "817",
                "signStatus": "NOT_ELIGIBLE",
                "signStatusDesc": null,
                "qualifiedDesc": "1.交割銀行為台新銀行。\r\n2.限可買賣交易證券戶，靜止戶及限制交易戶不適用。\r\n3.需留存聯絡電話及電子郵件信箱。",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_SIN",
                "itemName": "興櫃風險預告書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "SIN",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_W00",
                "itemName": "認購(售)權證【含國外標的,牛熊證,期信託,期商品】風險預告書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "W00",
                "signStatus": "SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_X01",
                "itemName": "指數股票型基金受益憑證買賣及申購買回特殊風險預告書(統一FANG+)",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "X01",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            },
            {
                "singKind": 1,
                "signId": "RY308_X02",
                "itemName": "富邦VIX指數股票型期貨信託基金受益憑證買賣及申購買回風險預告書",
                "desc": "* 當日 14:00 前簽署，次交易日生效",
                "apiKindId": "X02",
                "signStatus": "NOT_SIGNED",
                "signStatusDesc": null,
                "qualifiedDesc": "",
                "mappingSignStatus": null,
                "mappingSignId": null
            }
        ]
    }
    ```