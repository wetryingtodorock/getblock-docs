---
title: etc:txpool_besuStatistics \[POST\]
description: Lists statistics about the node transaction pool.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "txpool_besuStatistics",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "maxSize": 4096,
        "localCount": 1,
        "remoteCount": 0
    }
}
```

