---
title: eth:priv_uninstallFilter  {disallowed} - Ethereum
description: Example code for the eth:priv_uninstallFilter  {disallowed} ws method. Сomplete guide on how to use eth:priv_uninstallFilter  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`data` - None

Filter ID.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_uninstallFilter",
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

