---
title: bsv:preciousblock \[POST\]
description: Treats a block as if it were received before others with the same work.A later preciousblock call can override the effect of an earlier one.The effects of preciousblock are not retained across restarts.
---

### Parameters


`blockhash` - string, required

the hash of the block to mark as precious

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "preciousblock",
"params": ["000000000000000000046b9302e08c16ea186950f42a5498320ddd1bd7ab3428"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```

