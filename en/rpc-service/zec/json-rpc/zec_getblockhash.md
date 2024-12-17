---
title: zec:getblockhash \[POST\]
description: Returns hash of block in best-block-chain at index provided.
---

### Parameters


`index` - numeric

The block index. If negative then -1 is the last known valid block.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockhash",
"params": [1384123],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "0000000000938f9fc631767d1302cd7a2cc29fce45f82724eb4d55d11658768f"
}
```

