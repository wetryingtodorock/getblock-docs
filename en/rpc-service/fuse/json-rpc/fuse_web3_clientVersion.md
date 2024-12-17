---
title: web3_clientVersion - Fuse Network
description: Example code for the web3_clientVersion json-rpc method. Сomplete guide on how to use web3_clientVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
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
    "result": "OpenEthereum//v3.3.5-stable/x86_64-linux-musl/rustc1.59.0"
}
```

