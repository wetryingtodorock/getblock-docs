---
title: btc:getmemoryinfo - Bitcoin
description: Example code for the btc:getmemoryinfo json-rpc method. Сomplete guide on how to use btc:getmemoryinfo json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`mode` - string, optional, default=”stats”

Determines what kind of information is returned.

\- "stats" returns general statistics about memory usage in the daemon.

\- "mallocinfo" returns an XML string describing low-level heap state
(only available if compiled with glibc 2.10+).

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getmemoryinfo",
"params": [null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "locked": {
            "chunks_free": 1,
            "chunks_used": 1,
            "free": 65296,
            "locked": 65536,
            "total": 65536,
            "used": 240
        }
    }
}
```

