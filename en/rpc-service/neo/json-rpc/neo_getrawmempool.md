---
title: neo:getrawmempool \[POST\]
description: Obtains a list of confirmed / unconfirmed transactions in memory.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getrawmempool",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        "0x9786cce0dddb524c40ddbdd5e31a41ed1f6b5c8a683c122f627ca4a007a7cf4e",
        "0xb488ad25eb474f89d5ca3f985cc047ca96bc7373a6d3da8c0f192722896c1cd7",
        "0xf86f6f2c08fbf766ebe59dc84bc3b8829f1053f0a01deb26bf7960d99fa86cd6"
    ]
}
```

