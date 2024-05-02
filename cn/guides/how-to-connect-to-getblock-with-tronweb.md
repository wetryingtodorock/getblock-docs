---
lastUpdated: October 23, 2023
title: How to connect to GetBlock with TronWeb
description: Connect TronWeb to GetBlock effortlessly with our comprehensive guide. Access Tron blockchain data, interact with smart contracts, and optimize your Tron dApp development.
---

# 如何使用 TronWeb 連接到 GetBlock

TronWeb是TRON全節點API函數的JavaScript庫，用於部署智能合約、查詢區塊鍊和合約信息、在去中心化交易所進行交易以及改變區塊鏈狀態。 在本指南中，我們將向您展示如何開始使用 TronWeb 連接到 GetBlock。

首先，您需要將 TronWeb 庫添加到您的項目中。

- Npm: ```npm install tronweb```
- Yarn: ```yarn add tronweb```

首先，在您的 javascript 文件中定義 TronWeb：
```const TronWeb = require('tronweb');```

當您實例化 TronWeb 時，您可以定義：

- fullNode
- solidityNode
- eventServer
- privateKey

您還可以設置

- fullHost

這很有趣。 不過，如果您這樣做，則優先考慮更精確的規範。 假設您正在使用提供一切的服務器，例如 TronGrid，您可以將 TronWeb 實例化為：

```javascript
const tronWeb = new TronWeb({
fullHost: "https://go.getblock.io/<ACCESS-TOKEN>/"
})
```

不過，為了向後兼容，您可以繼續使用舊方法，其中任何參數都單獨傳遞（此處使用 GetBlock 節點作為示例）：

```javascript
const fullNode = new TronWeb.providers.HttpProvider("https://go.getblock.io/<ACCESS-TOKEN>/")
const solidityNode = new TronWeb.providers.HttpProvider("https://go.getblock.io/<ACCESS-TOKEN>/")
const eventServer = new TronWeb.providers.HttpProvider("https://go.getblock.io/<ACCESS-TOKEN>/")
const tronWeb = new TronWeb(fullNode, solidityNode, eventServer)
```

之後你可以調用任何 TronWeb 方法：

```javascript
tronWeb.trx.getBlock('latest').then(result => {console.log(result)});
```

![screenshot 1](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-tronweb/tronweb_screenshot.webp)

所有 API 參考都可以在 [https://developers.tron.network/reference](https://developers.tron.network/reference) 的項目文檔中找到

## 方法響應：

![screenshot 2](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-tronweb/tronweb_screenshot_1.webp)
