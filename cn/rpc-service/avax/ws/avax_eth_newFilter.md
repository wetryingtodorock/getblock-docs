---
title: avax:eth_newFilter \[WebSocket\]
description: Creates a filter object, based on filter options, to notify when thestate changes (logs). To check if the state has changed, calleth_getFilterChanges.A note on specifying topic filtersTopics are order-dependent. A transaction with a log with topics \[A,B\] will be matched by the following topic filters\[\] “anything”\[A\] “A in first position (and anything after)”\[null, B\] “anything in first position AND B in second position (andanything after)”\[A, B\] “A in first position AND B in second position (and anythingafter)”\[\[A, B\], \[A, B\]\] “(A OR B) in first position AND (A OR B) insecond position (and anything after)”
---

### Parameters


`Object` - object

Filter options

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newFilter",
"params": [{"fromBlock": "earliest", "toBlock": "latest", "topics": []}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x149c3e3f7a44b70568d865d6fd58c619"
}
```

