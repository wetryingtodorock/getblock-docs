---
title: dgb:getblockhash \[POST\]
description: Returns hash of block in best-block-chain at height provided.
---

### Parameters


`height` - numeric, required

The height index

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockhash",
"params": [13627174],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "8aef53e812659444b72dfa021ccbfddfb795e04889788c8dee802113e186acf3"
}
```

