---
title: btc:getaddednodeinfo \[POST\] {disallowed}
description: Returns information about the given added node, or all added nodes (notethat onetry addnodes are not listed here)
---

### Parameters


`node` - string, optional, default=all nodes

If provided, return information about this specific node, otherwise all
nodes are returned.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
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

