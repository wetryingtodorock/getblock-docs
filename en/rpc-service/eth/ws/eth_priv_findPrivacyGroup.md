---
title: priv_findPrivacyGroup  {disallowed} - Ethereum
description: Example code for the priv_findPrivacyGroup  {disallowed} ws method. Сomplete guide on how to use priv_findPrivacyGroup  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`array of data` - None

Members specified by Orion public keys.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_findPrivacyGroup",
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

