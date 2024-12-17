---
title: bsc:eth_gasPrice - Binance Smart Chain
description: Example code for the bsc:eth_gasPrice json-rpc method. Сomplete guide on how to use bsc:eth_gasPrice json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_gasPrice",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xb2d05e00"
}
```

