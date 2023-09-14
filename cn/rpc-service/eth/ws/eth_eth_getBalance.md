---
title: eth:eth_getBalance \[WebSocket\]
description: Returns the account balance of the specified address.
---

### Parameters


`DATA` - None

20-byte account address from which to retrieve the balance.

`QUANTITY|TAG` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xfe3b557e8fb62b89f4916b721be55ceb828dbd73", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x36ea"
}
```

