---
lastUpdated: October 24, 2023
title: 如何設置帳戶
description: 按照簡單的註冊流程，為您的共用或專用節點建立無限的端點。 追蹤您的請求、餘額和統計數據，並在需要時從 GetBlock 團隊獲取協助。
---

# 如何設置帳戶

要開始使用 GetBlock 節點連接服務來構建去中心化應用程序 (dApp)，需要註冊並定制一個帳戶。 只需點擊幾下！

## 步驟 1. 註冊 GetBlock

請選擇首選的註冊選項：

- 連接錢包。 通過選擇此選項，您無需共享您的電子郵件地址並創建新密碼。 如果您當前沒有錢包瀏覽器擴展程序，系統會要求您安裝該擴展程序。
- 使用 Google 登錄。 Google 將與 getblock.io 分享您的姓名、電子郵件地址、語言偏好和個人資料圖片。
- 使用電子郵件註冊。 您將被要求提供您的姓名和電子郵件地址。 如果您選擇第一個選項，系統會要求您驗證輸入的電子郵件地址。

請注意，要開始使用我們的服務，您將被要求接受我們的[服務條款](https://getblock.io/terms-of-service/)和[隱私政策](https://getblock.io/cn/privacy-policy/) -政策/）。

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

## 步骤 5. 了解共享节点的订阅

GetBlock 将客户的应用程序连接到 50 多个区块链 RPC 节点。

每次您的软件（钱包、dApp、加密货币交易所等）通过 GetBlock 基础设施与区块链交互时，该交互称为“请求”。 例如，您可以请求区块链通过哈希值显示区块详细信息，通过地址显示账户余额等。

为了开始向 GetBlock 的共享节点发送请求，用户可以选择“开始”订阅（请求数量有限）和“无限制”订阅。 此外，还提供 24 小时内 40,000 个请求的免费计划。

对于付费订阅，用户每月可以购买 5 到 1 亿个请求。 激活该时段的订阅后，未使用的请求可以转移到下一时段。

![screenshot 12](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_12.png)

例如，如果 Alice 在 10 月 10 日支付了 1 个月的订阅费用，并有 5000 万个请求，则该订阅将于 11 月 10 日到期。 如果她没有使用全部 5000 万个请求，则在她支付下一个周期的费用后，剩余的请求将变得可用。

此外，如果她认为 5000 万个请求不足以实现她的目标，她可以在仪表板中购买额外的包。

用户可以通过 Puddle 用法定货币支付订阅费用； 默认情况下设置定期付款以自动执行付款流程。 此外，客户还可以通过 Coinbase 用加密货币为账户充值； 可以一次性付款。 如果卡内余额不足，GetBlock会在三天内尝试再次充值，然后冻结请求。

以下计算有助于确定“开始”订阅的全部请求量在最大容量设置为每秒 200 个请求 (RpS) 时花费的时间：

- 5,000,000 个请求/（200 RpS * 60 秒）= 416 分钟（或 6 小时 57 分钟）；
- 10,000,000 个请求 / (200 RpS * 60 秒) = 833 分钟（或 13 小时 53 分钟）；
- 50,000,000 个请求/（200 RpS * 60 秒）= 4166 分钟（或 69 小时 27 分钟）；
- 100,000,000 个请求/（200 RpS * 60 秒）= 8332 分钟（或 138 小时 54 分钟）。

“无限制”计划用户可以在 1、3、6、9 或 12 个月内，在所有共享节点上以 300 RpS 的无与伦比的带宽访问无限数量的请求。

要与共享节点交互，请选择所需的协议和网络，单击“获取”，然后在几秒钟内收到您的端点地址和 API 令牌。

![screenshot 12](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_13.png)

请注意，您对共享节点的请求余额分布在“共享节点”选项卡下添加的所有端点上。

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
