---
title: getBlockTime - Solana
description: Example code for the getBlockTime json-rpc method. Сomplete guide on how to use getBlockTime json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`block` - u64

block, identified by Slot.

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBlockTime",
"params": [122791192],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 1646011316
}
```

