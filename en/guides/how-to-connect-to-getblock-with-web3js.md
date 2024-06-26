---
lastUpdated: October 23, 2023
title: How to connect to GetBlock with Web3.js
description: Discover how to seamlessly integrate Web3.js with GetBlock using our detailed guide. Access blockchain data, interact with smart contracts, and enhance your dApp development.
---

# How to connect to GetBlock with Web3.js

Web3.js is a JavaScript library built for interacting with the Ethereum blockchain. It is used to send JSON-RPC calls to the Ethereum node via HTTP, IPC or WebSocket connection in order to read data from the blockchain, make transactions or deploy smart contracts.

In this guide, we will show you how to get started with web3.js to connect to GetBlock. First of all, you will need to add web3.js library to your project. This can be done using the following commands:

- Npm: ```npm install web3```
- Yarn: ```yarn add web3```
- Pure js link: link the ```dist/web3.min.js```

After that you need to create a web3 instance and set a provider.

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

All API references can be found in the project documentation at [https://web3js.readthedocs.io](https://web3js.readthedocs.io/).

## Method response:

![screenshot 1](https://storage.getblock.io/web/docs/guides/how-to-connect-to-getblock-with-web3js/web3js_screenshot_1.webp)
