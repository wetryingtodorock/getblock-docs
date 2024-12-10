---
title: arbitrum:eth_blockNumber - Arbitrum
description: Example code for the arbitrum:eth_blockNumber json-rpc method. Сomplete guide on how to use arbitrum:eth_blockNumber json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://arbitrum.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_blockNumber",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x5bc406c"
}
```

