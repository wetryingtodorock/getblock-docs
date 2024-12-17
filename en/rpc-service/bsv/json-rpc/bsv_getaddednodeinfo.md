---
title: bsv:getaddednodeinfo  {disallowed} - Bitcoin SV
description: Example code for the bsv:getaddednodeinfo  {disallowed} json-rpc method. Сomplete guide on how to use bsv:getaddednodeinfo  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`node` - string, optional, default=all nodes

If provided, return information about this specific node, otherwise all
nodes are returned.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddednodeinfo",
"params": [null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

