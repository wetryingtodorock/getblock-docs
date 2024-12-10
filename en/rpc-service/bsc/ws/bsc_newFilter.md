---
title: bsc:newFilter  {disallowed} - Binance Smart Chain
description: Example code for the bsc:newFilter  {disallowed} ws method. Сomplete guide on how to use bsc:newFilter  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`to` - DATA

60 Bytes - (optional) Identity of the receiver. When present it will try
to decrypt any incoming message if the client holds the private key to
this identity.

`topics` - Array of DATA

Array of DATA topics which the incoming message's topics should match.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "newFilter",
"params": [null, null],
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

