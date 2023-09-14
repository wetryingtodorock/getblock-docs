---
lastUpdated: June 10, 2023
---

# 開始使用 GetBlock 公共 API

>如果您在這個頁面上 - 恭喜您，您只需幾分鐘即可深入了解我們的開發人員 API，每天有 40,000 個免費請求。 您所需要做的就是設置一個帳戶。

### 如何設立賬戶？

要在 GetBlock 上設置帳戶，您需要單擊右上角的“帳戶”按鈕 [主頁](https://getblock.io/) 或關注 [這個鏈接](https://account.getblock.io/sign-in).

### 步驟 1. 註冊 GetBlock

請選擇首選的註冊選項：

1. 連接錢包。 通過選擇此選項，您無需共享您的電子郵件地址並創建新密碼。 如果您當前沒有錢包瀏覽器擴展程序，系統會要求您安裝該擴展程序。
2. 使用 Google 登錄。 Google 將與 getblock.io 分享您的姓名、電子郵件地址、語言偏好和個人資料圖片。
3. 使用電子郵件註冊。 您將被要求提供您的姓名和電子郵件地址。 如果您選擇第一個選項，系統會要求您驗證輸入的電子郵件地址。

請注意，要開始使用我們的服務，您將被要求接受我們的 [服務條款](https://getblock.io/terms-of-service/) 和[隱私政策](https://getblock.io/privacy-policy/).

![screenshot 1](https://storage.getblock.io/web/docs/explorer-api/get-started/screenshot_1.webp)

### 步驟 2. 檢查您的用戶 ID。

在“帳戶設置”部分找到您的用戶 ID。 請在聯繫 GetBlock 團隊時使用它，以便我們識別您的帳戶並更快地為您提供幫助。

![screenshot 2](https://storage.getblock.io/web/docs/explorer-api/get-started/screenshot_2.webp)

### 第 3 步：確定 API 訪問權限。

在“選擇協議”中選擇“NEAR協議”，然後在接下來的“選擇網絡”選項卡中單擊“主網”。 您還可以從帳戶的主頁找到您的 API 密鑰。

![screenshot 3](https://storage.getblock.io/web/docs/explorer-api/get-started/screenshot_3.webp)

### 步驟 4. 了解請求包。

在“帳戶設置”部分中，您將在“請求餘額”按鈕下找到可用的定價計劃。 您還可以點擊賬戶主頁右上角的“添加”來查看計劃。 免費計劃包括每個帳戶每日 40,000 次請求的限制。 未使用的請求無法轉移到第二天，因此會丟失。

當您的應用程序訪問某個區塊鏈（發送令牌、驗證網絡狀態等）時，稱為“請求”。 您可以在“啟動”、“構建”、“擴展”和“無限制”選項之間進行選擇。

“啟動”、“構建”和“擴展”計劃是按使用付費的選項。 即使 30 天內未使用，購買的請求也不會被銷毀。

以下計算有助於確定在最大容量設置為每秒 60 個請求 (RpS) 的情況下，來自特定包的全部請求量將花費的時間：

- **“啟動”包**：5 000 000 個請求/（60 RpS * 60 秒）= 1 388 分鐘（或 23 小時 8 分鐘）；
- **“構建”包**：10 000 000 個請求/（60 RpS * 60 秒）= 2 777 分鐘（或 46 小時 17 分鐘）；
- **“規模”包**：50 000 000 個請求/（60 RpS * 60 秒）= 13 888 分鐘（或 9 天 15 小時 28 分鐘）。

通過“無限制”計劃，用戶可以在 30 天內訪問所有開發 API（現在僅 NEAR 可用）上無限數量的請求。

![screenshot 4](https://storage.getblock.io/web/docs/explorer-api/get-started/screenshot_4.webp)

### 步驟 5. 研究 GetBlock API 文檔

您可以在左側菜單中看到“NEAR Protocol Explorer”選項卡。 去那裡深入了解 GetBlock API 的工作原理以及它使用的方法。

![screenshot 5](https://storage.getblock.io/web/docs/explorer-api/get-started/screenshot_5.webp)

要使用 API，您需要將 API 密鑰粘貼到標有“x-api-key: YOUR-API-KEY”的“標題”行中。

### 第 6 步。瞧！ 您已準備好使用 API。

研究完文檔後，就可以開始您的開發之旅了！ 您每天有 40,000 個免費請求，您可以將它們用於任何用途。 它們也會每天更新，但未使用的請求不會轉移到第二天。 享受！
