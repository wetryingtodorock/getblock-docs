---
lastUpdated: October 23, 2023
title: How to connect to GetBlock with MetaMask
description: Learn how to connect MetaMask to GetBlock using our step-by-step guide. Ensure seamless integration and enjoy access to blockchain data to enhance your dApp development.
---

# How to connect to GetBlock with MetaMask

MetaMask is a browser extension that serves as an Ethereum wallet and enables you to run Ethereum dApps in a browser without running a full Ethereum node. It’s supported in Chrome, Brave, and Safari browsers.

To get started with MetaMask, you will need to install its extension for your smartphone or browser at [https://metamask.io/download](https://metamask.io/download). For Opera browser you can use “Install Chrome extensions” official add-on to install MetaMask from Chrome webstore.

Setup your wallet if you haven't done it yet.

To add Custom RPC Network click on the current network.

![screenshot 1](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-metamask/metamask_screenshot.webp)

Then click on the Custom RPC button.

![screenshot 2](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-metamask/metamask_screenshot_1.webp)

After this fill in the following fields:

- Network name – call it whatever you want; 
- New RPC URL – ```https://go.getblock.io/<ACCESS_TOKEN>/```;
- Chain ID – you can get Chain ID with this curl command:

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

- Currency Symbol – optional;
- Block Explorer – optional.

Then click on the Save button

![screenshot 3](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-metamask/metamask_screenshot_2.webp)

Custom network will be added and selected as default.
