---
title: eth_newBlockFilter - Cronos
description: Example code for the eth_newBlockFilter json-rpc method. Сomplete guide on how to use eth_newBlockFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
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
    "result": "0xf25654f61a34ac7b4e1222967b03dc1f"
}
```
