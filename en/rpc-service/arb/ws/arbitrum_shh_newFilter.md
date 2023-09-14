---
title: arbitrum:shh_newFilter \[WebSocket\] {disallowed}
description: Creates filter to notify, when client receives whisper message matchingthe filter options.
---

### Parameters


`filters` - json object

filter object: { "to": "address" (string, optional) - Identity of the
receiver. When present it will try to decrypt any incoming message if
the client holds the private key to this identity. "topics": \["topic"\]
(array of string) - Array of topics which the incoming message’s topics
should match. }

### Request

``` java
wscat -c wss://arbitrum.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_newFilter",
"params": [null],
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

