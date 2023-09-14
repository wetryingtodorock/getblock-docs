---
title: dash:masternode_current \[POST\] {disallowed}
description: Deprecated in Dash Core 0.17.0This RPC has been deprecated and will be removed in a future version ofDash CorePrints info on current masternode winner to be paid the next block(calculated locally).
---

### Parameters


`method name` - string

None

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "masternode",
"params": ["current"],
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

