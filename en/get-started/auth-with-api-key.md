---
lastUpdated: October 24, 2023
title: Authentication with API Key
description: Discover the steps for using the API key in the path string or as part of the x-api-key request header to ensure uninterrupted access to all GetBlock functionality.
---

# Authentication with API Key

**Note: This authentication method is deprecated and will be disabled on February 1st, 2024.**

You can still find your API-key based endpoints in the “Migration Required” section. Choose a project (each has its own API key) and access all previously created endpoints within the project. Please migrate them to access tokens as soon as possible to ensure uninterrupted access to all GetBlock functionality.

All endpoints contain API key in the path string. Your requests cannot be processed without the API key, and you will receive a 400 Bad Request error with the response body "Apikey missed."

You can authenticate with the API key using two methods, both of which work the same way:

Send API key in the path string:

```https://<SYMBOL>.getblock.io/YOUR-API-KEY/mainnet/```

Copy the API key from the project Dashboard and paste it to the x-api-key request header:

```
Host:<SYMBOL>.getblock.io/mainnet/
x-api-key:YOUR-API-KEY
```

Each node has its own set of methods for interacting with the blockchain network. You can find the methods for several nodes in the "Available Nodes Methods" tab in the Documentation.

### How to send requests to a node (ex. Ethereum and Bitcoin)

The Ethereum node supports JSON-RPC and WebSockets interfaces, while the Bitcoin node – REST and JSON-RPC. You can access the connection using such command-line utilities as cURL and wscat, and also various libraries built for interaction with certain blockchains. The guides on how to connect to GetBlock with [Web3.js](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-web3js/), [TronWeb](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-tronweb/) and [MetaMask](https://getblock.io/docs/guides/how-to-connect-to-getblock-with-metamask/) are provided in Documentation.

### Wscat

If you want to send data requests with WebSockets, you can use several libraries or wscat. You can install and use wscat as follows:

- Download wscat from [https://www.npmjs.com/package/wscat](https://www.npmjs.com/package/wscat)
- Install wscat by running the following command: ```npm install -g wscat```

You can connect to the Ethereum node with wscat using two options:
1. Recommended.\
```wscat -c 'wss://eth.getblock.io/mainnet/' --header 'x-api-key: <Api key>'```
2. ```wscat -c 'wss://eth.getblock.io/mainnet/?api_key=<Api key>'```

When the command is performed, you will get a response inside the terminal that the connection is successfully enabled.
