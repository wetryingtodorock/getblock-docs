---
lastUpdated: October 23, 2023
title: How to connect to GetBlock with MetaMask
description: Learn how to connect MetaMask to GetBlock using our step-by-step guide. Ensure seamless integration and enjoy access to blockchain data to enhance your dApp development.
---

# 如何使用 MetaMask 連接到 GetBlock

MetaMask 是一個瀏覽器擴展，可用作以太坊錢包，使您能夠在瀏覽器中運行以太坊 dApp，而無需運行完整的以太坊節點。 Chrome、Brave 和 Safari 瀏覽器均支持它。

要開始使用 MetaMask，您需要在 [https://metamask.io/download](https://metamask.io/download) 上為您的智能手機或瀏覽器安裝其擴展程序。 對於 Opera 瀏覽器，您可以使用“安裝 Chrome 擴展”官方插件從 Chrome 網上商店安裝 MetaMask。

如果您還沒有設置您的錢包，請先設置它。

要添加自定義 RPC 網絡，請單擊當前網絡。

![screenshot 1](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-metamask/metamask_screenshot.webp)

然後單擊自定義 RPC 按鈕。

![screenshot 2](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-metamask/metamask_screenshot_1.webp)

之後填寫以下字段：

- 網絡名稱 – 隨意命名；
- 新的 RPC URL – ```https://go.getblock.io/<ACCESS_TOKEN>/```；
- 鏈 ID – 您可以使用以下curl 命令獲取鏈 ID：

```shell
curl --location --request POST 'https://go.getblock.io/<ACCESS-TOKEN>/' \
--header 'Content-Type: application/json' \
--data-raw '{
  "jsonrpc": "2.0",
  "method": "eth_chainId",
  "params": [],
  "id": "getblock.io"
}'
```

- 貨幣符號 – 可選；
- 區塊瀏覽器 – 可選。

然後單擊“保存”按鈕

![screenshot 3](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-metamask/metamask_screenshot_2.webp)

將添加自定義網絡並選擇默認網絡。
