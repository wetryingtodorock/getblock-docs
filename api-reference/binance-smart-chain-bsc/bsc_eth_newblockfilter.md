---
title: eth_newBlockFilter - Binance Smart Chain
description: Example code for the eth_newBlockFilter json-rpc method. Сomplete guide on how to use eth_newBlockFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xffd6440dfd893a0fa29a0e506e153de8"
}
```
