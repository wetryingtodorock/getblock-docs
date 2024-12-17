---
title: priv_deletePrivacyGroup  {disallowed} - Ethereum
description: Example code for the priv_deletePrivacyGroup  {disallowed} ws method. Сomplete guide on how to use priv_deletePrivacyGroup  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Privacy group ID

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_deletePrivacyGroup",
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

