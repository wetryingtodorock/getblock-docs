---
title: bsv:abortrescan \[POST\] {disallowed}
description: Stops current wallet rescan triggered by an RPC call, e.g. by animportprivkey call. Note Use getwalletinfo to query the scanningprogress.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "abortrescan",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

