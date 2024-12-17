---
title: zec:getaddednodeinfo \[POST\] {disallowed}
description: Returns information about the given added node, or all added nodes.If dns is false, only a list of added nodes will be provided, otherwiseconnected information will also be available.
---

### Parameters


`dns` - boolean

If false, only a list of added nodes will be provided, otherwise
connected information will also be available.

`node` - string

Optional.

If provided, return information about this specific node, otherwise all
nodes are returned.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddednodeinfo",
"params": [null, null],
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

