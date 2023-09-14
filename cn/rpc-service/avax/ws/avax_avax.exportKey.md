---
title: avax:avax.exportKey \[WebSocket\] {disallowed}
description: Get the private key that controls a given address. The returned privatekey can be added to a user with avax.importKey.
---

### Parameters


`username` - string

username must control address.

`password` - string

user's password

`address` - string

address is the address for which you want to export the corresponding
private key.

It should be in hex format.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.exportKey",
"params": [null, null, null],
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

