---
title: ksm:chain_subscribeAllHeads - Kusama
description: Example code for the ksm:chain_subscribeAllHeads json-rpc method. Сomplete guide on how to use ksm:chain_subscribeAllHeads json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "chain_subscribeAllHeads",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32603,
        "message": "Internal error"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

