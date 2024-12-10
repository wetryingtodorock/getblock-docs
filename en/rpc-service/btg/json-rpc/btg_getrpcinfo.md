---
title: btg:getrpcinfo - Bitcoin Gold
description: Example code for the btg:getrpcinfo json-rpc method. Сomplete guide on how to use btg:getrpcinfo json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
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
                "method": "getrpcinfo",
                "duration": 35
            }
        ],
        "logpath": "/coin/data/debug.log"
    }
}
```

