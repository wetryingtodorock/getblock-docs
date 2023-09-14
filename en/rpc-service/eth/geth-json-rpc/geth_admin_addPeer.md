---
title: geth:admin_addPeer \[POST\] {disallowed}
description: The addPeer administrative method requests adding a new remote node tothe list of tracked static nodes. The node will try to maintainconnectivity to these nodes at all times, reconnecting every once in awhile if the remote connection goes down.
---

### Parameters


`url` - string

The enode URL of the remote peer to start tracking and returns a BOOL
indicating whether the peer was accepted for tracking or some error
occurred.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_addPeer",
"params": ["peerurl"],
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

