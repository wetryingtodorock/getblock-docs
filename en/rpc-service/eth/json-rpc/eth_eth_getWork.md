---
title: eth:eth_getWork \[POST\]
description: Returns the hash of the current block, the seed hash, and the requiredtarget boundary condition.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getWork",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "no mining work available yet"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

