---
title: matic:eth_newPendingTransactionFilter - Polygon
description: Example code for the matic:eth_newPendingTransactionFilter json-rpc method. Сomplete guide on how to use matic:eth_newPendingTransactionFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newPendingTransactionFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x5f1f04c3bd761f5c9f47d541cd4f5eec"
}
```

