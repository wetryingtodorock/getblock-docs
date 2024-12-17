---
title: btc:addnode \[POST\] {disallowed}
description: Attempts to add or remove a node from the addnode list.Or try a connection to a node once.Nodes added using addnode (or -connect) are protected from DoSdisconnection and are not required to be full nodes/support SegWit asother outbound peers are (though such peers will not be synced from).
---

### Parameters


`node` - string, required

The node (see getpeerinfo for nodes)

`command` - string, required

‘add’ to add a node to the list, ‘remove’ to remove a node from the
list, ‘onetry’ to try a connection to the node once

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
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

