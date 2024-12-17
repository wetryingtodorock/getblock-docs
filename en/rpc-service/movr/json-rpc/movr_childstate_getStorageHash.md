---
title: movr:childstate_getStorageHash \[POST\] {disallowed}
description: Returns the hash of a child storage entry at a block state.
---

### Parameters


`childKey` - PrefixedStorageKey

None

`key` - StorageKey

None

`at` - Hash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "childstate_getStorageHash",
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

