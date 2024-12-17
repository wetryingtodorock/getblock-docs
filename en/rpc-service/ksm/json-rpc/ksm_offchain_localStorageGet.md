---
title: ksm:offchain_localStorageGet \[POST\] {disallowed}
description: Get offchain local storage under given key and prefix.
---

### Parameters


`kind` - StorageKind

None

`key` - Bytes

None

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "offchain_localStorageGet",
"params": [null, null],
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

