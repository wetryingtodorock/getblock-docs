---
title: neo:getstateroot \[POST\]
description: Queries the state root by the block height.
---

### Parameters


`index` - numeric

Block index

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getstateroot",
"params": [7902013],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "flag": "Unverified",
        "stateroot": {
            "index": 7902013,
            "prehash": "0xeedae97fc591eb483ad52048d4d10639602f413edaaff9caafaabbfebffd0680",
            "stateroot": "0x0277d10c5332cf5e34d09d392f8bd9beb7e5dda7b7861572df8784b164f86976",
            "version": 0,
            "witness": {}
        }
    }
}
```

