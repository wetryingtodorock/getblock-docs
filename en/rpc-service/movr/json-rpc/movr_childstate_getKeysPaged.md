---
title: movr:childstate_getKeysPaged \[POST\] {disallowed}
description: Returns the keys with prefix from a child storage with paginationsupport.
---

### Parameters


`childKey` - PrefixedStorageKey

None

`prefix` - StorageKey

None

`count` - u32

None

`startKey` - StorageKey

None

`at` - Hash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "childstate_getKeysPaged",
"params": [null, null, null, null, null],
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

