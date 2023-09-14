---
title: geth:admin_peers \[POST\] {disallowed}
description: The peers administrative property can be queried for all the informationknown about the connected remote nodes at the networking granularity.These include general information about the nodes themselves asparticipants of the ÐΞVp2p P2P overlay protocol, as well as specializedinformation added by each of the running application protocols (e.g.eth, les, shh, bzz).
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_peers",
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

