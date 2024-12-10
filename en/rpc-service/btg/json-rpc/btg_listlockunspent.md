---
title: btg:listlockunspent  {disallowed} - Bitcoin Gold
description: Example code for the btg:listlockunspent  {disallowed} json-rpc method. Сomplete guide on how to use btg:listlockunspent  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listlockunspent",
"params": [],
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

