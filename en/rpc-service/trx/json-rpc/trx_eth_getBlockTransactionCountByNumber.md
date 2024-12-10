---
title: trx:eth_getBlockTransactionCountByNumber - TRON
description: Example code for the trx:eth_getBlockTransactionCountByNumber json-rpc method. Сomplete guide on how to use trx:eth_getBlockTransactionCountByNumber json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - QUANTITY

Integer of a block number, or the string "earliest", "latest"

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
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
    "result": "0x95"
}
```

