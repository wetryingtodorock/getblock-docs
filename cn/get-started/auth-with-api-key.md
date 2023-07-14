---
lastUpdated: June 10, 2023
---

# 使用 API 密鑰進行身份驗證

創建帳戶並登錄後，您將被帶到 GetBlock 儀表板。 在那裡您會找到一個自動生成的 API 密鑰——與服務交互和發出 API 請求所需的令牌。

![screenshot 1](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_1.webp)

如果需要，您可以創建多個 API 密鑰。 只需按下位於您的 API 密鑰旁邊的塊中的“創建新的 API 密鑰”鏈接。

![screenshot 2](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_2.webp)

輸入新 API 密鑰的名稱，然後在彈出窗口中按“創建”按鈕。

![screenshot 3](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_3.webp)

新的 API 密鑰將顯示在前一個 API 密鑰的旁邊。

![screenshot 4](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_4.webp)

接收到的 API 密鑰是向我們的區塊鏈節點發送請求所必需的。 如果沒有 API 密鑰，您的請求將無法處理，您將收到響應正文“Apikey missed”的 ```400 Bad Request``` 錯誤。

您可以使用兩種方法使用 API 密鑰進行身份驗證：

### 推薦方法
從儀表板複製 API 密鑰並將其粘貼到 ```x-api-key``` 請求標頭：

```
Host:<SYMBOL>.getblock.io/mainnet/
x-api-key:YOUR-API-KEY
```

### API 密鑰也可以在查詢字符串中發送：
```
https://<SYMBOL>.getblock.io/mainnet/?api_key=YOUR-API-KEY
```

每個節點都有自己的一套與區塊鍊網絡交互的方法。 您可以在文檔的 RPC 服務選項卡中找到多個節點的方法。

如果你找不到你需要的節點的方法，你總是可以在 [節點端點](https://getblock.io/docs/nodes-endpoints/) 單擊位於節點端點旁邊的所需 API 接口（JSON-RPC、REST 或 WS）按鈕。

![screenshot 5](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_5.webp)


### 如何向節點發送請求（例如以太坊和比特幣）

以太坊節點支持 JSON-RPC 和 WebSockets 接口，而比特幣節點支持 REST 和 JSON-RPC。 您可以使用 cURL 和 wscat 等命令行實用程序以及為與某些區塊鏈交互而構建的各種庫來訪問連接。 有關如何連接到 GetBlock 的指南 [Web3.js](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-web3js/), [TronWeb](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-tronweb/) 和 [MetaMask](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-metamask/) 在文檔中提供。

### Wscat

如果你想用 WebSockets 發送數據請求，你可以使用幾個庫或 wscat。 您可以按如下方式安裝和使用 wscat：

