---
title: geth:admin_removePeer \[POST\] {disallowed}
description: Disconnects from a remote node if the connection exists.It returns a boolean indicating validations succeeded. Note a true valuedoesn’t necessarily mean that there was a connection which wasdisconnected.
---

### Parameters


`url` - string

The enode url of a peer to be disconnected.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_removePeer",
"params": ["encode.url"],
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

