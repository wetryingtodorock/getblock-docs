---
title: geth:txpool_status \[POST\]
description: The status inspection property can be queried for the number oftransactions currently pending for inclusion in the next block(s), aswell as the ones that are being scheduled for future execution only.The result is an object with two fields pending and queued, each ofwhich is a counter representing the number of transactions in thatparticular state.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
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
        "pending": "0x13fd",
        "queued": "0x400"
    }
}
```

