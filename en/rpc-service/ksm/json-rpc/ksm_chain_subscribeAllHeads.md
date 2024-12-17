---
title: ksm:chain_subscribeAllHeads \[POST\]
description: Retrieves the newest header via subscription.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "chain_subscribeAllHeads",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32603,
        "message": "Internal error"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

