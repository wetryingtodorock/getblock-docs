---
lastUpdated: October 23, 2023
title: How to connect to GetBlock with Web3.js
description: Discover how to seamlessly integrate Web3.js with GetBlock using our detailed guide. Access blockchain data, interact with smart contracts, and enhance your dApp development.
---

# 如何使用 Web3.js 連接到 GetBlock

Web3.js 是一個為與以太坊區塊鏈交互而構建的 JavaScript 庫。 它用於通過 HTTP、IPC 或 WebSocket 連接向以太坊節點發送 JSON-RPC 調用，以便從區塊鏈讀取數據、進行交易或部署智能合約。

在本指南中，我們將向您展示如何開始使用 web3.js 連接到 GetBlock。 首先，您需要將 web3.js 庫添加到您的項目中。 這可以使用以下命令來完成：

- Npm: ```npm install web3```
- Yarn: ```yarn add web3```
- 純js鏈接：鏈接 ```dist/web3.min.js```

之後，您需要創建一個 web3 實例並設置提供程序。

```javascript
// In case you are using Node.js
const Web3 = require('web3');
// Setting getblock node as HTTP provider
const provider = new Web3.providers.HttpProvider("https://go.getblock.io/<ACCESS-TOKEN>/");
// or as WebSocket provider
const provider = new Web3.providers.WebsocketProvider("wss://go.getblock.io/<ACCESS-TOKEN>/");
// Creating web3 instance with given provider
const web3 = new Web3(provider);
// Initializing web3.eth method
var block = web3.eth.getBlockNumber().then(console.log);
```

![screenshot 1](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-web3js/web3js_screenshot.webp)

所有 API 參考都可以在 [https://web3js.readthedocs.io](https://web3js.readthedocs.io/) 的項目文檔中找到。

## 方法響應：

![screenshot 2](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-web3js/web3js_screenshot_1.webp)
