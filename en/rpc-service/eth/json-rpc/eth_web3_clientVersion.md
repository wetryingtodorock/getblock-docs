---
title: eth:web3_clientVersion - Ethereum
description: Example code for the eth:web3_clientVersion json-rpc method. Сomplete guide on how to use eth:web3_clientVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "web3_clientVersion",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "Geth/v1.11.6-stable-ea9e62ca/linux-amd64/go1.20.3"
}
```

