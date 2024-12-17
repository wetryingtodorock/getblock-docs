---
title: matic:eth_getBalance \[WebSocket\]
description: Returns the balance of the account of given address.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xe7e2cb8c81c10ff191a73fe266788c9ce62ec754", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x14bf15b14d996e4b7eb8"
}
```

