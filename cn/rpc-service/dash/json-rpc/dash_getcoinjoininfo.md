---
title: dash:getcoinjoininfo \[POST\]
description: Returns an object containing an information about CoinJoin settings andstate (previously named getprivatesendinfo prior to Dash Core 0.17.0).
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getcoinjoininfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "denoms_goal": 50,
        "denoms_hardcap": 300,
        "enabled": false,
        "max_amount": 1000,
        "max_rounds": 4,
        "max_sessions": 4,
        "multisession": false,
        "queue_size": 0
    }
}
```

