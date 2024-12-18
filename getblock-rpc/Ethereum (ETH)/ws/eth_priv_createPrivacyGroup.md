---
title: priv_createPrivacyGroup  {disallowed} - Ethereum
description: Example code for the priv_createPrivacyGroup  {disallowed} ws method. Сomplete guide on how to use priv_createPrivacyGroup  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - None

Request options

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_createPrivacyGroup",
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

