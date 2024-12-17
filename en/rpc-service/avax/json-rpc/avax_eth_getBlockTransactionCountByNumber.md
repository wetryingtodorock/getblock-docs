---
title: avax:eth_getBlockTransactionCountByNumber \[POST\]
description: Returns the number of transactions in a block matching the given blocknumber.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByNumber",
"params": ["latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x8"
}
```

