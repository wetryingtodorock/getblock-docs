---
title: geth:admin_peerEvents \[POST\] {disallowed}
description: PeerEvents creates an RPC subscription which receives peer events fromthe node’s p2p server.The type of events emitted by the server are as follows add emittedwhen a peer is added drop emitted when a peer is dropped msgsendemitted when a message is successfully sent to a peer msgrecv emittedwhen a message is received from a peer
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_peerEvents",
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

