
# Eplatfrom Api Spec Index
 
- [e櫃登入](#eplatfromLogin)
  - [Step1.雷影登入(此時還未取得權限)](#loginStep1)
    - [雷影登入](./ePlatformApiSepc/%E7%99%BB%E5%85%A5/%E9%9B%B7%E5%BD%B1%E7%99%BB%E5%85%A5.md)
    - [TrustLogin](./ePlatformApiSepc/%E7%99%BB%E5%85%A5/Trust%20login%2083ec4ac47f944428a38d3bd3a0f918e0.md)
  - [Step2.驗章(成功頒發權限)](./ePlatformApiSepc/%E7%99%BB%E5%85%A5/%E9%A9%97%E7%AB%A0.md)
- [取得Refresh Token](./ePlatformApiSepc/%E5%8F%96%E5%BE%97RefreshToken.md)
- [取得ClientIP](./ePlatformApiSepc/%E5%8F%96%E5%BE%97ClientIP.md)
- [驗證碼相關](#captcha)
  - [取得驗證碼](./ePlatformApiSepc/%E9%A9%97%E8%AD%89%E7%A2%BC%E7%9B%B8%E9%97%9C/%E5%8F%96%E5%BE%97%E9%A9%97%E8%AD%89%E7%A2%BC.md)
  - [驗證驗證碼](./ePlatformApiSepc/%E9%A9%97%E8%AD%89%E7%A2%BC%E7%9B%B8%E9%97%9C/%E9%A9%97%E8%AD%89%E9%A9%97%E8%AD%89%E7%A2%BC.md)
- [修改密碼](./ePlatformApiSepc/%E4%BF%AE%E6%94%B9%E5%AF%86%E7%A2%BC.md)
- [密碼暫不變更通知](./ePlatformApiSepc/%E5%AF%86%E7%A2%BC%E6%9A%AB%E4%B8%8D%E8%AE%8A%E6%9B%B4%E9%80%9A%E7%9F%A5.md)
- [密碼解鎖](#passwordLock)
    - [Step1 輸入身份證、生日](./ePlatformApiSepc/%E5%AF%86%E7%A2%BC%E8%A7%A3%E9%8E%96/Step1%20%E8%BC%B8%E5%85%A5%E8%BA%AB%E4%BB%BD%E8%AD%89%E3%80%81%E7%94%9F%E6%97%A5.md)
    - [Step2 產生OTP](./ePlatformApiSepc/%E5%AF%86%E7%A2%BC%E8%A7%A3%E9%8E%96/Step2%20%E7%94%A2%E7%94%9FOTP.md)
    - [Step3 驗證OTP](./ePlatformApiSepc/%E5%AF%86%E7%A2%BC%E8%A7%A3%E9%8E%96/Step3%20%E9%A9%97%E8%AD%89OTP.md)
- [公告](#announce)
  - [取得輪播公告](./ePlatformApiSepc/%E5%85%AC%E5%91%8A/%E5%8F%96%E5%BE%97%E8%BC%AA%E6%92%AD%E5%85%AC%E5%91%8A.md)
  - [取得登入前登入後公告](./ePlatformApiSepc/%E5%85%AC%E5%91%8A/%E5%8F%96%E5%BE%97%E7%99%BB%E5%85%A5%E5%89%8D%E7%99%BB%E5%85%A5%E5%BE%8C%E5%85%AC%E5%91%8A.md)
  - [取得登入前登入後特定公告(單筆)](./ePlatformApiSepc/%E5%85%AC%E5%91%8A/%E5%8F%96%E5%BE%97%E7%99%BB%E5%85%A5%E5%89%8D%E7%99%BB%E5%85%A5%E5%BE%8C%E7%89%B9%E5%AE%9A%E5%85%AC%E5%91%8A(%E5%96%AE%E7%AD%86).md)
- [活動輪播](./ePlatformApiSepc/%E6%B4%BB%E5%8B%95%E8%BC%AA%E6%92%AD/%E5%8F%96%E5%BE%97%E6%B4%BB%E5%8B%95%E8%BC%AA%E6%92%AD.md)
- [服務據點](#branchOffice)
  - [取得所有分行](./ePlatformApiSepc/%E6%9C%8D%E5%8B%99%E6%93%9A%E9%BB%9E/%E5%8F%96%E5%BE%97%E6%89%80%E6%9C%89%E5%88%86%E8%A1%8C.md)
  - [取得特定類型分行](./ePlatformApiSepc/%E6%9C%8D%E5%8B%99%E6%93%9A%E9%BB%9E/%E5%8F%96%E5%BE%97%E7%89%B9%E5%AE%9A%E9%A1%9E%E5%9E%8B%E5%88%86%E8%A1%8C.md)
- [停站公告](./ePlatformApiSepc/%E5%81%9C%E7%AB%99%E5%85%AC%E5%91%8A.md)
- [聲明宣告](./ePlatformApiSepc/%E8%81%B2%E6%98%8E%E5%AE%A3%E5%91%8A-%E9%9A%B1%E7%A7%81%E6%AC%8A.md)
- [OTP驗證碼](#OTPCaptcha)
  - [產生OTP驗證碼](./ePlatformApiSepc/OTP%E9%A9%97%E8%AD%89%E7%A2%BC/%E7%94%A2%E7%94%9FOTP%E9%A9%97%E8%AD%89%E7%A2%BC.md)
  - [驗證OTP驗證碼](./ePlatformApiSepc/OTP%E9%A9%97%E8%AD%89%E7%A2%BC/%E9%A9%97%E8%AD%89OTP%E9%A9%97%E8%AD%89%E7%A2%BC.md)
- [簽署中心](#signCenter)
  - [簽署列表](#signList)
    - [查詢單類型signKind](./ePlatformApiSepc/%E7%B0%BD%E7%BD%B2%E4%B8%AD%E5%BF%83/%E7%B0%BD%E7%BD%B2%E5%88%97%E8%A1%A8%20(%E6%9F%A5%E8%A9%A2%E5%96%AE%E9%A1%9E%E5%9E%8BsignKind).md)
    - [查詢多類型](./ePlatformApiSepc/%E7%B0%BD%E7%BD%B2%E4%B8%AD%E5%BF%83/%E7%B0%BD%E7%BD%B2%E5%88%97%E8%A1%A8%20(%E6%9F%A5%E8%A9%A2%E5%A4%9A%E9%A1%9E%E5%9E%8B).md)
    - [查詢標籤](./ePlatformApiSepc/%E7%B0%BD%E7%BD%B2%E4%B8%AD%E5%BF%83/%E7%B0%BD%E7%BD%B2%E5%88%97%E8%A1%A8(%E6%9F%A5%E8%A9%A2%E6%A8%99%E7%B1%A4).md)
  - [取得簽署標籤定義列表](./ePlatformApiSepc/%E7%B0%BD%E7%BD%B2%E4%B8%AD%E5%BF%83/%E5%8F%96%E5%BE%97%E7%B0%BD%E7%BD%B2%E6%A8%99%E7%B1%A4%E5%AE%9A%E7%BE%A9%E5%88%97%E8%A1%A8.md)
  - [簽署條文](./ePlatformApiSepc/%E7%B0%BD%E7%BD%B2%E4%B8%AD%E5%BF%83/%E7%B0%BD%E7%BD%B2%E6%A2%9D%E6%96%87.md)
  - [簽署](./ePlatformApiSepc/%E7%B0%BD%E7%BD%B2%E4%B8%AD%E5%BF%83/%E7%B0%BD%E7%BD%B2.md)


# ePlatform Api Sepc

Domain: [http://testecounter.tssco.com.tw/eplatform/api](http://testecounter.tssco.com.tw/eplatform/api)




