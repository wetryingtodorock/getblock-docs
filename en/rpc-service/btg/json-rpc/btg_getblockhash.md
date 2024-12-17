---
title: btg:getblockhash \[POST\]
description: Returns hash of block in best-block-chain at height provided.
---

### Parameters


`height` - numeric, required

The height index

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockhash",
"params": [702518],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "000000009ec5dd6b53858593718cacdaaec989aaf9028c68013947224712682e"
}
```

