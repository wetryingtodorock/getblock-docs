---
title: bch:getnodeaddresses \[POST\] {disallowed}
description: Return known addresses which can potentially be used to find new nodesin the network
---

### Parameters


`count` - numeric, optional, default=1

How many addresses to return. Limited to the smaller of 2500 or 23% of
all known addresses.

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getnodeaddresses",
"params": [null],
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

