---
title: sol:getTransactionCount - Solana
description: Example code for the sol:getTransactionCount json-rpc method. Сomplete guide on how to use sol:getTransactionCount json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`commitment` - object

Optional

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getTransactionCount",
"params": [null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 60547116336
}
```

