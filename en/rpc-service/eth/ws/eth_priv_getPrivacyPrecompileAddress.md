---
title: eth:priv_getPrivacyPrecompileAddress \[WebSocket\] {disallowed}
description: Returns the address of the privacy precompiled contract. The address isderived and based on the value of the privacy-onchain-groups-enabledoption.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getPrivacyPrecompileAddress",
"params": [],
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

