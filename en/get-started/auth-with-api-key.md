---
lastUpdated: June 10, 2023
---

# Authentication with API Key

Once you have created an account and signed in, you will be taken to the GetBlock Dashboard. There you will find an automatically generated first project that has a unique API key – a token required for interacting with the service and making API requests.

![screenshot 1](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/new_screenshot_1.png)

You can create several projects if needed. Simply press the “+” button in the “My projects” section and enter a name for a new project.

![screenshot 2](https://storage.getblock.io/web/docs/get-started/auth-with-api-key/new_screenshot_2.png)

To send requests to our blockchain nodes, create an endpoint in the chosen project. Endpoints created in different projects will contain different API keys. Endpoints are created with the API key in the path string. Your requests cannot be processed without the API key, and you will receive a 400 Bad Request error with the response body "Apikey missed."

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