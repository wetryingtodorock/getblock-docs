---
title: fuse:eth_coinbase \[POST\]
description: Returns the client coinbase address.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32023,
        "data": "\"\"",
        "message": "No accounts were found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```
