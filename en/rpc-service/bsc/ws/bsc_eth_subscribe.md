---
title: bsc:eth_subscribe \[WebSocket\]
description: Subscribes to a specified event type, optionally restricted to one ormany objects. This method is available via websocket only.
---

### Parameters


`type` - string

A subscription type, such as newHeads (new headers appended to the
chain, including chain reorganizations), logs (logs that are included in
new imported blocks and match the given filter criteria) or
newPendingTransactions (hashes for all transactions that are added to
the pending state and are signed with a key that is available in the
node).

`objects` - hex string

Optional argumants such as an address, multiple addresses, and topics.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_subscribe",
"params": ["newHeads", null],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": "0xe5af64ddfd365b4632988c5935cfedb7"
}
```

