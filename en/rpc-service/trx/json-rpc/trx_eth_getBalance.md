---
title: trx:eth_getBalance - TRON
description: Example code for the trx:eth_getBalance json-rpc method. Сomplete guide on how to use trx:eth_getBalance json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - bytes

address to check for balance.

`QUANTITY` - string

currently, only "latest" is available.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0x30760c7e10b1d3509d8d64a7e9eb9ab94bc83495", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x863b9dd3d1f"
}
```

