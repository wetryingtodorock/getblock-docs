---
title: btc:setnetworkactive \[POST\] {disallowed}
description: Disable/enable all p2p network activity.
---

### Parameters


`state` - boolean, required

true to enable networking, false to disable

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "setnetworkactive",
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

