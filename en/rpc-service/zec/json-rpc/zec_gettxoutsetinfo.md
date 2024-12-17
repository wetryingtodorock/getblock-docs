---
title: zec:gettxoutsetinfo \[POST\]
description: Returns statistics about the unspent transaction output set.Note this call may take some time.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "gettxoutsetinfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "bestblock": "00000000019af1612080b8d6b3ce87c5b7569a114e6a77385260cf45a6419fe1",
        "bytes_serialized": 555247948,
        "hash_serialized": "f0d96a7b8e69c26c904d68a8edc52cbd4676188aa8b9e94504adb0957ffd256d",
        "height": 1384358,
        "total_amount": 10682341.70673279,
        "transactions": 1613584,
        "txouts": 20130753
    }
}
```

