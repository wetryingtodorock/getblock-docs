---
title: optimism:rpc_modules \[POST\]
description: Lists enabled APIs and the version of each.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "rpc_modules",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "debug": "1.0",
        "eth": "1.0",
        "net": "1.0",
        "rollup": "1.0",
        "rpc": "1.0",
        "web3": "1.0"
    }
}
```

