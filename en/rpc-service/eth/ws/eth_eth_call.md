---
title: eth:eth_call - Ethereum
description: Example code for the eth:eth_call ws method. Сomplete guide on how to use eth:eth_call ws in GetBlock.io Web3 documentation.
---

### Parameters


`OBJECT` - None

Transaction call object.

`QUANTITY|TAG` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_call",
"params": [{"to": "0x69498dd54bd25aa0c886cf1f8b8ae0856d55ff13", "value": "0x1"}, "latest"],
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

