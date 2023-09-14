---
title: eth:eth_getCode \[WebSocket\]
description: Returns the code of the smart contract at the specified address. Besustores compiled smart contract code as a hexadecimal value.
---

### Parameters


`DATA` - None

20-byte contract address.

`QUANTITY|TAG` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getCode",
"params": ["0xa50a51c09a5c451c52bb714527e1974b686d8e77", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x"
}
```

