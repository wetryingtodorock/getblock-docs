---
title: eth_getBlockByNumber  {disallowed} - Polkadot
description: Example code for the eth_getBlockByNumber  {disallowed} json-rpc method. Сomplete guide on how to use eth_getBlockByNumber  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`block` - BlockNumber

block nubmer

`full` - bool

full or not

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockByNumber",
"params": [null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

