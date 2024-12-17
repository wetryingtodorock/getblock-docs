---
title: etc:priv_getPrivacyPrecompileAddress \[POST\] {disallowed}
description: Returns the address of the privacy precompiled contract. The address isderived and based on the value of the privacy-onchain-groups-enabledoption.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getPrivacyPrecompileAddress",
"params": [],
"id": "getblock.io"}'
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

