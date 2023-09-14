---
title: trx:eth_getBlockTransactionCountByHash \[POST\]
description: Returns the number of transactions in a block from a block matching thegiven block hash.
---

### Parameters


`blockhash` - data, 32 bytes

hash of a block

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/fullnode/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByHash",
"params": ["0x00000000025ad523bf3d34c17ff81e2cf46824d38ff0373d172fd293ca7e651f"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xd6"
}
```

