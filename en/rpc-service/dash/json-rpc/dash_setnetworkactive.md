---
title: dash:setnetworkactive \[POST\] {disallowed}
description: Disables/enables all P2P network activity.
---

### Parameters


`Activate` - bool

Set to true to enable all P2P network activity.

Set to false to disable all P2P network activity

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
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

