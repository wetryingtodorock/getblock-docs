---
title: trx:eth_syncing \[POST\]
description: Returns an object with data about the sync status of the node
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_syncing",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "currentBlock": "0x25ad7ec",
        "highestBlock": "0x25ad7ed",
        "startingBlock": "0x25ad7d9"
    }
}
```

