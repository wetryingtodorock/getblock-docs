---
title: zec:zcrawjoinsplit \[POST\] {disallowed}
description: DEPRECATED. Splices a joinsplit into rawtx. Inputs are unilaterallyconfidential. Outputs are confidential between sender/receiver. Thevpub_old and vpub_new values are globally public and move transparentvalue into or out of the confidential value store, respectively.Note The caller is responsible for delivering the output enc1 and enc2to the appropriate recipients, as well as signing rawtxout and ensuringit is mined. (A future RPC call will deliver the confidential paymentsin-band on the blockchain.)
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "zcrawjoinsplit",
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

