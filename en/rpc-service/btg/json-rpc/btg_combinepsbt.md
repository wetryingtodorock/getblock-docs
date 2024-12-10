---
title: btg:combinepsbt - Bitcoin Gold
description: Example code for the btg:combinepsbt json-rpc method. Сomplete guide on how to use btg:combinepsbt json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`txs` - json array, required

A json array of base64 strings of partially signed transactions

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "combinepsbt",
"params": [["mybase64_1", "mybase64_2", "mybase64_3"]],
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

