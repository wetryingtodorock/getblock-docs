---
title: trx:eth_getStorageAt \[POST\]
description: Returns the value from a storage position at a given address. It can beused to get the value of a variable in a contract.
---

### Parameters


`DATA` - 20 bytes

address

`QUANTITY` - integer

integer of the position in the storage

`QUANTITY|TAG` - string

currently, only "latest" is available.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0x30760c7e10b1d3509d8d64a7e9eb9ab94bc83495", "0x0", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0000000000000000000000000000000000000000000000000000000000000000"
}
```

