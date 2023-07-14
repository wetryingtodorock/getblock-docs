---
lastUpdated: June 10, 2023
---

# 如何設置帳戶

要開始使用 GetBlock 節點連接服務來構建去中心化應用程序 (dApp)，需要註冊並定制一個帳戶。 只需點擊幾下！

## 步驟 1. 註冊 GetBlock

請選擇首選的註冊選項：

1.連接錢包。 通過選擇此選項，您無需共享您的電子郵件地址並創建新密碼。 如果您當前沒有錢包瀏覽器擴展程序，系統會要求您安裝該擴展程序。

2. 使用 Google 登錄。 Google 將與 getblock.io 分享您的姓名、電子郵件地址、語言偏好和個人資料圖片。

3. 使用電子郵件註冊。 您將被要求提供您的姓名和電子郵件地址。 如果您選擇第一個選項，系統會要求您驗證輸入的電子郵件地址。

請注意，要開始使用我們的服務，您將被要求接受我們的[服務條款](https://getblock.io/terms-of-service/)和[隱私政策](https://getblock.io/privacy) -政策/）。

![screenshot 1](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_1.webp)

## 步驟 2. 檢查您的用戶 ID。

在“帳戶設置”部分找到您的用戶 ID。 請在聯繫 GetBlock 團隊時使用它，以便我們識別您的帳戶並更快地為您提供幫助。

![screenshot 2](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_2.webp)

## 步驟 3. 選擇與區塊鏈交互的方式

通過[共享節點](https://getblock.io/nodes/)，用戶可以訪問對等共享節點基礎設施。 此選項非常適合早期分散式應用程序。

- 訪問 50 多個連鎖店
- 速率限制：60 個請求/秒
- 提供按使用付費選項

[專用節點](https://getblock.io/dedicated-nodes/)作為GetBlock託管的私有服務，保證Web3開發解決方案的簡單集成和各種dApp的無縫啟動。 專用節點的端點不從賬戶餘額中收取費用。

- 無速率限制（每秒 1000 個以上請求，具體取決於區塊鏈）
- 99.9% 的可用性
- 自定義設置

在每個端點旁邊的下拉列表中選擇要用於與區塊鏈交互的 API 接口。 根據協議的不同，可以使用多種 API 接口（JSON-RPC、REST、WS 等）。

![screenshot 3](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_3.webp)

## 步驟4.創建共享節點或專用節點項目

登錄到您的帳戶。 您將看到包含您的項目的基本儀表板。 每個項目都會顯示一個唯一的 API 密鑰，可以在右上角找到。

使用 GetBlock 帳戶，您可以為共享節點和專用節點創建無限數量的項目。 請注意，一個項目不能同時用於共享節點和專用節點：

1. 要創建[共享節點](https://getblock.io/nodes/)項目，請按“我的項目”部分中的“+”按鈕。 根據需要向該項目添加任意數量的共享端點。 您對共享節點的請求餘額分佈在標有“共享節點”代碼的所有項目上。
2. 要創建[專用節點](https://getblock.io/dedicated-nodes/)項目，請配置專用節點並在選擇項目時選擇“新建”。 該項目將在部署第一個專用節點後立即創建。 您可以稍後向項目添加更多專用節點。

![screenshot 4](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_4.webp)

## 步驟5.了解共享節點的請求包

GetBlock 提供各種區塊鏈服務，包括訪問 50 多個領先網絡的節點。

在“帳戶設置”部分，您將找到可用的定價計劃。 免費計劃包括每個帳戶每日 40,000 次請求的限制。 未使用的請求無法轉移到第二天，因此會丟失。

當您的應用程序訪問某個區塊鏈（發送令牌、驗證網絡狀態等）時，稱為“請求”。 您可以在“啟動”、“構建”、“擴展”和“無限制”選項之間進行選擇。

“啟動”、“構建”和“擴展”計劃是按使用付費的選項。 即使 30 天內未使用，購買的請求也不會被銷毀。

以下計算有助於確定在最大容量設置為每秒 60 個請求 (RpS) 的情況下，來自特定包的全部請求量將花費的時間：

- **“啟動”包**：5 000 000 個請求/（60 RpS * 60 秒）= 1 388 分鐘（或 23 小時 8 分鐘）；

- **“構建”包**：10 000 000 個請求/（60 RpS * 60 秒）= 2 777 分鐘（或 46 小時 17 分鐘）；

- **“規模”包**：50 000 000 個請求/（60 RpS * 60 秒）= 13 888 分鐘（或 9 天 15 小時 28 分鐘）。

通過“無限制”計劃，用戶可以在 30 天內在所有共享節點上訪問無限數量的請求。

![screenshot 5](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_5.webp)

要與共享節點交互，請選擇所需的協議和網絡，單擊“獲取”，然後在幾秒鐘內收到您的端點鏈接。

請注意，您對共享節點的請求餘額分佈在標記為“共享節點”的所有項目上。

您可以使用“請求限制”按鈕為每個項目設置自定義請求限制。 該限制將應用於項目內的所有端點。

## 步驟 6. 配置專用節點

您可以按照簡單的分步過程來配置專用節點，首先選擇要部署的協議：

![screenshot 6](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_6.webp)

接下來您要做的就是選擇一個計劃（自動應用可用折扣）並設置您的私人定制 API 端點。

通過 GetBlock 帳戶支付專用節點費用，或在必要時選擇客戶支持選項。

## 步驟 7. 研究 GetBlock 文檔

![screenshot 7](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_7.webp)

深入了解 [GetBlock 的工作原理](https://getblock.io/docs/)、它使用哪些方法以及區塊鏈節點提供商如何與節點交互。

## 步驟 8. 創建對節點的請求

要連接到區塊鏈節點，請從您的帳戶檢索端點並將其插入到您的應用程序中。 每個端點都包含您項目的 API 密鑰。 請確保在路徑中傳遞您的 API 密鑰。 您還可以在標頭中傳遞您的 API 密鑰； 如果需要的話。

**確保您的 API 密鑰安全存儲。**

![screenshot 8](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_8.webp)

您還可以下載Postman GetBlock的[合集](https://documenter.getpostman.com/view/12951625/TWDTNKP9)來測試我們的服務。 找到所需的節點名稱並插入 API 密鑰。

![screenshot 9](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_9.webp)

連接建立後，用戶可以檢查他/她的請求歷史記錄。

此外，用戶可以通過命令行界面 (CLI) 訪問他/她的連接。 例如，以下是如何通過 GetBlock CLI 驗證幣安智能鏈（BSC）主網的高度。

![screenshot 10](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_10.webp)

## 步驟 9. 檢查請求統計信息

要查看統計數據，請選擇區塊鏈名稱和分析數據的確切時間段。

![screenshot 11](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_11.webp)

將顯示所有請求。 如果您使用多個節點，該信息也可以單獨以信息圖表的形式提供。

請繼續關注 GetBlock 團隊直接發布的更多更新和公告。
