---
title: matic:eth_protocolVersion \[POST\]
description: Returns the current ethereum protocol version.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_protocolVersion",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method eth_protocolVersion does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

