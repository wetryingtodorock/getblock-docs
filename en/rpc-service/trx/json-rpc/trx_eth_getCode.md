---
title: trx:eth_getCode \[POST\]
description: Returns runtime code of a given smart contract address.
---

### Parameters


`address` - DATA, 20 bytes

contract address

`QUANTITY|TAG` - string

currently, only "latest" is available.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getCode",
"params": ["0x30760c7e10b1d3509d8d64a7e9eb9ab94bc83495", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x"
}
```

