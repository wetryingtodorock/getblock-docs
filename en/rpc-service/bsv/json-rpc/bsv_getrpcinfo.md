---
title: bsv:getrpcinfo \[POST\]
description: Returns details of the RPC server.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getrpcinfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "active_commands": [
            {
                "duration": 72,
                "method": "getrpcinfo"
            }
        ],
        "logpath": "/home/bitcoin/.bitcoin/debug.log"
    }
}
```

