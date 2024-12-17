---
title: ftm:txpool_status - Fantom
description: Example code for the ftm:txpool_status json-rpc method. Сomplete guide on how to use ftm:txpool_status json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "txpool_status",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "pending": "0xb8",
        "queued": "0x100"
    }
}
```

