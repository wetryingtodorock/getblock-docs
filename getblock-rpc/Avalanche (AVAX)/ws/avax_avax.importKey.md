---
title: avax.importKey  {disallowed} - Avalanche
description: Example code for the avax.importKey  {disallowed} ws method. Сomplete guide on how to use avax.importKey  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`username` - string

user name

`password` - string

user password

`privateKey` - string

private key

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.importKey",
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

