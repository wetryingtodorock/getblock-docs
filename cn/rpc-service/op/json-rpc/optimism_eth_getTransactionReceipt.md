---
title: optimism:eth_getTransactionReceipt \[POST\]
description: Returns the receipt of a transaction by transaction hash.Note That the receipt is not available for pending transactions.
---

### Parameters


`DATA` - string

Hash of a transaction.

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionReceipt",
"params": ["0xb036e4ff7e7f596615d121d3a1c923c618bd3c2d3745c512346d7d8e583f01f7"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```

