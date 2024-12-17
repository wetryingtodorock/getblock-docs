---
title: zec:addnode \[POST\] {disallowed}
description: Attempts to add or remove a node from the addnode list. Or try aconnection to a node once.
---

### Parameters


`node` - string

The node.

`command` - string

"add" to add a node to the list, "remove" to remove a node from the
list, "onetry" to try a connection to the node once

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "addnode",
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

