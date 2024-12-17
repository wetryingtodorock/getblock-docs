---
title: trx:eth_getBlockTransactionCountByHash - TRON
description: Example code for the trx:eth_getBlockTransactionCountByHash json-rpc method. Сomplete guide on how to use trx:eth_getBlockTransactionCountByHash json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockhash` - data, 32 bytes

hash of a block

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \
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

