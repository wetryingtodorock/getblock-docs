---
title: fuse:eth_getBlockTransactionCountByHash \[POST\]
description: Returns the number of transactions in a block from a block matching thegiven block hash.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByHash",
"params": ["0x360c79467da57c8db35624484cabbca4d9fc7a7813f194f5391639d2e2c39023"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```

