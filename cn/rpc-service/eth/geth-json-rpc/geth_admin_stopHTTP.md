---
title: geth:admin_stopHTTP \[POST\] {disallowed}
description: The stopHTTP administrative method closes the currently open HTTP RPCendpoint. As the node can only have a single HTTP endpoint running, thismethod takes no parameters, returning a boolean whether the endpoint wasclosed or not.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_stopHTTP",
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

