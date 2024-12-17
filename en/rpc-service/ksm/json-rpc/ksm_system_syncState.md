---
title: ksm:system_syncState \[POST\]
description: Returns the state of the syncing of the node.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "system_syncState",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "currentBlock": 16049622,
        "highestBlock": 16049622,
        "startingBlock": 16032618
    }
}
```

