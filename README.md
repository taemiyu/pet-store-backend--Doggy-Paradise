# DoggyParadise寵物平台網站
這是一個結合寵物實體商店線下及線上資源的多系統平台，包含會員、商城、活動、旅館、動態牆。
>本寵物平台網站使用maven進行套件管理，以Spring Boot框架進行開發，並再application.properties檔中儲存專案執行所需的設定資料。相關設定請參考下方的開始。

## 環境
- MySQL:8.0.31
- JDK 17
## 功能特色

- 功能1：串接第3方API
    - Google OAuth2第三方登入
    - Line Pay、綠界支付
    - Google Gemini API
    - Cloudinary 線上雲端資料庫
     
- 功能2：開發風格
    - RESTful
    - 前後端分離
    - 後端三層式架構:dao、service、controller

## 快速開始

- 使用Spring Boot在Maven專案運行localhost 8080，Vue專案使用vite套件運行在localhost 5173。

- SQL Query位於DoogyParadise_SQL.sql，可直接於MySQL建置資料庫環境，員工須於資料庫自行新增一筆。

- application.properties與Google第三方登入的properties設定為application_properties_config.txt及google_OAuth2_config.txt，需自行設定(並放入專案resource資料夾中)。

- Google OAuth2第三方登入需要申請Google Cloud 第三方登入申請憑證(如果不想使用可以註解掉)。

- Google Gemini API:需自行去Google AI Studio申請API Key，截至2024/4月底前都是免費。

- Cloudinary 雲端圖片資料庫需自行註冊並使用其所配置的API Key。

- 網站內mail發信功能必須至google帳號開通二階段驗證與應用程式密碼。
