---
title: ksm:system_localListenAddresses \[POST\] {disallowed}
description: The addresses include a trailing /p2p/ with the local PeerId, and arethus suitable to be passed to addReservedPeer or as a bootnode addressfor example
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "system_localListenAddresses",
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

