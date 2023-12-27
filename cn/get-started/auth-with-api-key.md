---
lastUpdated: October 24, 2023
---

# 使用 API 金鑰進行身份驗證

**注意：此身份驗證方法已棄用，並將於 2024 年 2 月 1 日停用。**

您仍然可以在「需要遷移」部分找到基於 API 金鑰的端點。 選擇一個專案（每個專案都有自己的 API 金鑰）並存取該專案中先前建立的所有端點。 請盡快將它們遷移到存取令牌，以確保不間斷地存取所有 GetBlock 功能。

所有端點的路徑字串中都包含 API 金鑰。 如果沒有 API 金鑰，則無法處理您的請求，並且您將收到 400 錯誤請求錯誤，回應正文為「Apikey Missed」。

您可以使用兩種方法透過 API 金鑰進行身份驗證，這兩種方法的工作方式相同：

在路徑字串中傳送 API 金鑰：

```https://<SYMBOL>.getblock.io/YOUR-API-KEY/mainnet/```

從專案儀表板複製 API 金鑰並將其貼上到 x-api-key 請求標頭：

```
Host:<SYMBOL>.getblock.io/mainnet/
x-api-key:YOUR-API-KEY
```

每個節點都有自己的一套與區塊鏈網路互動的方法。 您可以在文件的「可用節點方法」標籤中找到多個節點的方法。

### 如何向節點發送請求（例如以太坊和比特幣）

以太坊節點支援 JSON-RPC 和 WebSockets 接口，而比特幣節點支援 REST 和 JSON-RPC。 您可以使用 cURL 和 wscat 等命令列實用程式以及為與某些區塊鏈互動而建立的各種庫來存取連接。 有關如何使用[Web3.js](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-web3js/)、[TronWeb](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-web3js/) 和 [MetaMask](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-metamask/) 在文件中提供。

### Wscat

如果要使用 WebSocket 傳送資料請求，可以使用多個庫或 wscat。 您可以如下安裝和使用 wscat：

- 從 [https://www.npmjs.com/package/wscat](https://www.npmjs.com/package/wscat) 下載 wscat
- 透過執行以下指令安裝 wscat：```npm install -g wscat```

您可以使用以下兩個選項透過 wscat 連接到以太坊節點：

1. 受到推崇的.\
   ```wscat -c 'wss://eth.getblock.io/mainnet/' --header 'x-api-key: <Api key>'```
2. ```wscat -c 'wss://eth.getblock.io/mainnet/?api_key=<Api key>'```

執行指令後，您將在終端機內收到連線已成功啟用的回應。
