---
title: sol:getBlockHeight - Solana
description: Example code for the sol:getBlockHeight json-rpc method. Сomplete guide on how to use sol:getBlockHeight json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Commitment` - object

Optional.

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBlockHeight",
"params": [null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 111246105
}
```

