---
title: kcc:shh_newFilter  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:shh_newFilter  {disallowed} ws method. Сomplete guide on how to use kcc:shh_newFilter  {disallowed} ws in GetBlock.io Web3 documentation.
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
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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

