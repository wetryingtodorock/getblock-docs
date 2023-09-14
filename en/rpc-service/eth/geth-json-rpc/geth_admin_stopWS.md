---
title: geth:admin_stopWS \[POST\] {disallowed}
description: The stopWS administrative method closes the currently open WebSocket RPCendpoint. As the node can only have a single WebSocket endpoint running,this method takes no parameters, returning a boolean whether theendpoint was closed or not.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_stopWS",
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

