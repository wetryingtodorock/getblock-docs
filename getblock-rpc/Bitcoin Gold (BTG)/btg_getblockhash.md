---
title: getblockhash - Bitcoin Gold
description: Example code for the getblockhash json-rpc method. Сomplete guide on how to use getblockhash json-rpc in GetBlock.io Web3 documentation.
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

