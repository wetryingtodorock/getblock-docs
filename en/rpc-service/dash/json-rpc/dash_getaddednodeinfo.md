---
title: dash:getaddednodeinfo \[POST\] {disallowed}
description: Returns information about the given added node, or all added nodes(except onetry nodes). Only nodes which have been manually added usingthe addnode RPC will have their information displayed.
---

### Parameters


`node` - string

Optional.

The node to get information about in the same IP_address:port format as
the addnode RPC. If this parameter is not provided, information about
all added nodes will be returned

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddednodeinfo",
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

