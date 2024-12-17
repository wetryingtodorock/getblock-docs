---
title: ont:getblockcount - Ontology
description: Example code for the ont:getblockcount json-rpc method. Сomplete guide on how to use ont:getblockcount json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockcount",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "desc": "SUCCESS",
    "error": 0,
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 16224578
}
```

