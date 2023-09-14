---
title: ksm:offchain_localStorageSet \[POST\] {disallowed}
description: Set offchain local storage under given key and prefix.
---

### Parameters


`kind` - StorageKind

None

`key` - Bytes

None

`value` - Bytes

None

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "offchain_localStorageSet",
"params": [null, null, null],
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

