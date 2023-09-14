---
title: doge:getinfo \[POST\]
description: Returns an ServerInfo object containing various state info.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getinfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "blocks": 3906176,
        "connections": 14,
        "difficulty": 4386136.832791463,
        "errors": "",
        "paytxfee": 1.0,
        "protocolversion": 70015,
        "proxy": "",
        "relayfee": 0.001,
        "testnet": false,
        "timeoffset": -1,
        "version": 1140400
    }
}
```

