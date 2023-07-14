---
lastUpdated: June 10, 2023
---

# Authentication with API Key

Once you created an account and signed in, you will be taken to the GetBlock Dashboard. There you will find an automatically generated API key – a token required for the interaction with the service and making API requests.

![screenshot 1](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_1.webp)

You can create several API keys if needed. Simply press the “Create new API Key” link in the block located next to your API key.

![screenshot 2](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_2.webp)

Enter the name for a new API key and press the “Create” button in the pop-up window.

![screenshot 3](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_3.webp)

The new API key will be displayed next to the previous one.

![screenshot 4](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_4.webp)

The received API keys are required for sending requests to our blockchain nodes. Your requests can’t be processed without the API key, you will receive the ```400 Bad Request``` error with the response body “Apikey missed”.

You can authenticate with the API key using two methods:

### Recommended method.
Copy the API key from the Dashboard and paste it to the ```x-api-key``` request header:

```
Host:<SYMBOL>.getblock.io/mainnet/
x-api-key:YOUR-API-KEY
```

### The API key can be also sent in the query string:
```
https://<SYMBOL>.getblock.io/mainnet/?api_key=YOUR-API-KEY
```

Each node has its own set of methods for interaction with the blockchain network. You can find methods for several nodes in the RPC Service tab in Documentation.

If you can’t find methods for the node you need, you can always find them in the [Nodes Endpoints](https://getblock.io/docs/nodes-endpoints/) section by clicking the required API interface (JSON-RPC, REST or WS) button located next to the endpoint of the node.

![screenshot 5](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/screenshot_5.webp)


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
