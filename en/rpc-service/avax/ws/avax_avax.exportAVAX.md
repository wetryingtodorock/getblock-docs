---
title: avax:avax.exportAVAX  {disallowed} - Avalanche
description: Example code for the avax:avax.exportAVAX  {disallowed} ws method. Сomplete guide on how to use avax:avax.exportAVAX  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`to` - string

the X-Chain address the asset is sent to.

`amount` - int

amount of the asset to send.

`baseFee` - int

base fee that should be used when creating the transaction. If ommitted,
a suggested fee will be used.

`username` - string

user that controls the address that transaction will be sent from.

`password` - string

user's password

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.exportAVAX",
"params": [null, null, null, null, null],
"id": "getblock.io"}
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

