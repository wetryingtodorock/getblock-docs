---
title: movr:state_getChildStorage \[POST\] {disallowed}
description: Retrieves the child storage for a key.
---

### Parameters


`childStorageKey` - StorageKey

child storage key

`childDefinition` - StorageKey

child storage key definition

`childType` - u32

child type

`key` - StorageKey

storage key

`at` - BlockHash

block hash

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "state_getChildStorage",
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

