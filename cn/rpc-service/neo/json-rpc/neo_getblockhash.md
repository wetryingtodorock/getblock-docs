---
title: neo:getblockhash \[POST\]
description: Returns the hash value of the corresponding block based on the specifiedindex.
---

### Parameters


`index` - numeric

Block index (block height)

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockhash",
"params": [7901859],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xf3372f6dbaf489c603c340fe8e225b3dc83c394b7667908ff45fc558eebb4477"
}
```

