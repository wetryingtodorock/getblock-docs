---
title: geth:admin_nodeInfo \[POST\] {disallowed}
description: The nodeInfo administrative property can be queried for all theinformation known about the running Geth node at the networkinggranularity. These include general information about the node itself asa participant of the ÐΞVp2p P2P overlay protocol, as well as specializedinformation added by each of the running application protocols (e.g.eth, les, shh, bzz).
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_nodeInfo",
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

