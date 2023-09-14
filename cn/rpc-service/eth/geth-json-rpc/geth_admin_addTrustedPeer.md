---
title: geth:admin_addTrustedPeer \[POST\] {disallowed}
description: Adds the given node to a reserved trusted list which allows the node toalways connect, even if the slots are full.It returns a BOOL to indicate whether the peer was successfully added tothe list.
---

### Parameters


`url` - string

The enode URL of the remote peer to start tracking.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_addTrustedPeer",
"params": ["remote.peer.url"],
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

