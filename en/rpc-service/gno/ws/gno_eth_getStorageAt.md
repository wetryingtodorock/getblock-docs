---
title: gno:eth_getStorageAt - Gnosis
description: Example code for the gno:eth_getStorageAt ws method. Сomplete guide on how to use gno:eth_getStorageAt ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

A 20-byte storage address.

`QUANTITY` - hex string

Integer index of the storage position.

`QUANTITY|TAG` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0x9EC55d57208cb28a7714A2eA3468bD9d5bB15125", "0x0", "latest"],
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

