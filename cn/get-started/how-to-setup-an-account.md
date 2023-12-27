---
lastUpdated: October 24, 2023
---

# 如何設置帳戶

要開始使用 GetBlock 節點連接服務來構建去中心化應用程序 (dApp)，需要註冊並定制一個帳戶。 只需點擊幾下！

## 步驟 1. 註冊 GetBlock

請選擇首選的註冊選項：

- 連接錢包。 通過選擇此選項，您無需共享您的電子郵件地址並創建新密碼。 如果您當前沒有錢包瀏覽器擴展程序，系統會要求您安裝該擴展程序。
- 使用 Google 登錄。 Google 將與 getblock.io 分享您的姓名、電子郵件地址、語言偏好和個人資料圖片。
- 使用電子郵件註冊。 您將被要求提供您的姓名和電子郵件地址。 如果您選擇第一個選項，系統會要求您驗證輸入的電子郵件地址。

請注意，要開始使用我們的服務，您將被要求接受我們的[服務條款](https://getblock.io/terms-of-service/)和[隱私政策](https://getblock.io/privacy) -政策/）。

![screenshot 1](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_1.webp)

## 步驟 2. 檢查您的用戶 ID。

在“帳戶設置”部分找到您的用戶 ID。 請在聯繫 GetBlock 團隊時使用它，以便我們識別您的帳戶並更快地為您提供幫助。

![screenshot 2](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_2.webp)

## 步驟 3. 選擇與區塊鏈交互的方式

通過[共享節點](https://getblock.io/nodes/)，用戶可以訪問對等共享節點基礎設施。 此選項非常適合早期分散式應用程序。

- 訪問 50 多個連鎖店
- 速率限制：200 個請求/秒
- 提供按使用付費選項

[專用節點](https://getblock.io/dedicated-nodes/)作為GetBlock託管的私有服務，保證Web3開發解決方案的簡單集成和各種dApp的無縫啟動。 專用節點的端點不從賬戶餘額中收取費用。

- 無速率限制（每秒 1000 個以上請求，具體取決於區塊鏈）
- 99.9% 的可用性
- 自定義設置

在每個端點旁邊的下拉列表中選擇要用於與區塊鏈交互的 API 接口。 根據協議的不同，可以使用多種 API 接口（JSON-RPC、REST、WS 等）。

![screenshot 3](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_3.webp)

## 步驟 4. 建立共用節點或專用節點端點

登入您的帳戶。 您將看到一個基本儀表板，其中包含端點和一般統計資料。
使用 GetBlock 帳戶，您可以為共用節點和專用節點建立無限數量的端點。

1. 若要建立[共用節點](https://getblock.io/nodes/)端點，請導覽至「儀表板」並向下捲動至「我的端點」部分。 選擇協定、網路和所需的 API。 根據需要向該協定添加任意數量的存取權杖。 您對共享節點的請求餘額分佈在標有「共享節點」代碼的所有項目上。
2. 若要建立[專用節點](https://getblock.io/dedicated-nodes/)端點，請切換至「專用節點」標籤。 選擇協定和可用網路。 點擊“獲取”以繼續從彈出的視窗中配置專用節點。 您可以按照以下步驟新增更多專用節點。 根據需要為每個專用節點添加盡可能多的存取令牌。

![screenshot 4](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_4.webp)

在每個協定或專用節點旁邊，您將找到一個關聯的設定檔。 展開端點以查看為協定產生的所有存取權杖。

## 步驟5.了解共享節點的請求包

GetBlock 提供各種區塊鏈服務，包括存取 50 多個領先網路的節點。

前往側邊欄中的「新增請求」標籤，尋找可用的定價方案。 免費方案包括每個帳戶每日 40,000 次請求的限制。 未使用的請求無法轉移到第二天，因此會遺失。

當您的應用程式存取某個區塊鏈（發送代幣、驗證網路狀態等）時，稱為「請求」。 您可以選擇“按請求付費”和“無限制存取”選項。

透過按使用付費選項，即使 30 天內未使用，購買的請求也不會被銷毀。

以下計算有助於確定「按請求付費」套件中的全部請求量在最大容量設定為每秒 60 個請求 (RpS) 時花費的時間：

- 5,000,000 個請求 / (200 RpS * 60 秒) = 416 分鐘（或 6 小時 57 分鐘)
- 10,000,000 個請求 / (200 RpS * 60 秒) = 833 分鐘（或 13 小時 53 分鐘）
- 50,000,000 個請求 / (200 RpS * 60 秒) = 4166 分鐘（或 69 小時 27 分鐘）

「無限制」計畫使用者可以在 1、6 或 12 個月內存取所有共享節點上的無限數量的請求。

![screenshot 5](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_5.webp)

要與共享節點交互，請選擇所需的協定和網絡，按一下“獲取”，然後在幾秒鐘內收到您的端點連結。

請注意，您對共享節點的請求餘額分佈在「共享節點」標籤下新增的所有端點上。

此外，您可以使用儀表板上的「Boost」按鈕增加共享節點的自訂速率限制。 一旦獲得批准，該限制將應用於所有共用端點。 請聯絡我們的支援團隊以獲取更多資訊。

## 步驟 6. 配置專用節點

您可以按照簡單的分步過程來配置專用節點，首先選擇要部署的協議：

![screenshot 6](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_6.webp)

接下來您要做的就是選擇一個計劃（自動應用可用折扣）並設置您的私人定制 API 端點。

通過 GetBlock 帳戶支付專用節點費用，或在必要時選擇客戶支持選項。

## 步驟 7. 研究 GetBlock 文檔

![screenshot 7](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_7.webp)

深入了解 [GetBlock 的工作原理](https://getblock.io/docs/)、它使用哪些方法以及區塊鏈節點提供商如何與節點交互。

## 步驟 8. 建立對節點的請求

若要連接到區塊鏈節點，請從儀表板複製包含存取權杖的端點，或檢索設定檔並將其匯入到您的應用程式中。

確保您的存取令牌的安全儲存。 如果遭到洩露，存取令牌可以輕鬆滾動或刪除。 按下受感染端點旁的“...”按鈕，然後選擇所需的選項。

您可以選擇單獨下載每個協定的設定檔。 這些檔案將包含 JSON 和 JS 格式的特定端點的所有存取權杖。 要一次取得所有存取令牌，只需點擊「我的端點」旁邊的檔案圖示即可。

如果需要，您可以為選定的區塊鏈或專用節點設定多個存取權杖。

![screenshot 8](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_8.webp)

您也可以下載Postman GetBlock的[合集](https://documenter.getpostman.com/view/28751185/2s9YRDzqcX#ca02e504-8079-48e2-9bf0-d0a022b43774)來測試我們的服務。

![screenshot 9](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_9.webp)

連線建立後，使用者可以檢查其請求的歷史記錄。

此外，使用者還可以透過命令列介面 (CLI) 存取其連線。 例如，以下是如何透過 GetBlock CLI 驗證幣安智能鏈（BSC）主網的高度。

![screenshot 10](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_10.webp)

## 步驟 9. 檢查請求統計訊息

要檢查統計信息，請前往“我的端點”部分並切換到“統計信息”選項卡。 您可以使用下拉式選單按參數或令牌自訂資料視圖。

選擇時間段、區塊鏈名稱、網路和 API 來分析數據。

![screenshot 11](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_11.webp)

所有關於請求數量、回應狀態、方法呼叫和速率限制拒絕的資訊都將以資訊圖表的形式顯示。

請繼續關注 GetBlock 團隊直接發布的更多更新和公告。
