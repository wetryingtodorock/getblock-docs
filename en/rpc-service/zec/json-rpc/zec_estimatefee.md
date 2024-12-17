---
title: zec:estimatefee - Zcash
description: Example code for the zec:estimatefee json-rpc method. Сomplete guide on how to use zec:estimatefee json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`nblocks` - numeric

None

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "estimatefee",
"params": [5],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": 0.0001005
}
```

