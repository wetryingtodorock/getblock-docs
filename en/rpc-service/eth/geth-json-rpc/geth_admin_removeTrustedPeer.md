---
title: geth:admin_removeTrustedPeer \[POST\] {disallowed}
description: Removes a remote node from the trusted peer set, but it does notdisconnect it automatically.It returns a boolean indicating validations succeeded.
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
"method": "admin_removeTrustedPeer",
"params": ["encode.peer.url"],
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

