---
title: geth:debug_storageRangeAt \[POST\] {disallowed}
description: Returns the storage at the given block height and transaction index. Theresult can be paged by providing a maxResult to cap the number ofstorage slots returned as well as specifying the offset via keyStart(hash of storage key).
---

### Parameters


`blockHash` - string

hash of a block

`txIx` - int

None

`contractAddress` - string

None

`keyStart` - string

hash of storage key

`maxResult` - int

max results per page

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_storageRangeAt",
"params": ["0x63a0e8e7c9e86cf58e188b98f55cedee42c3c902", 1, "0x97a363e191f1f01459b2a9987edd7c01c962f4ce", "0xe3962f0c7b342e3517a7a6e1a8c6ab51565840d93ca457caf462358ff2e612c", 5],
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

