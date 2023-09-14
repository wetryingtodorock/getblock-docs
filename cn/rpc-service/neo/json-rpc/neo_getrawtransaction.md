---
title: neo:getrawtransaction \[POST\]
description: Returns the corresponding transaction information based on the specifiedhash value.
---

### Parameters


`txid` - string

Transaction ID

`verbose` - bool or numeric, optional, default=false

When verbose is false, serialized information of the block is returned
in a Base64-encoded string. If you need the detailed information, use
the SDK for deserialization.

When verbose is true or 1, detailed information of the block is returned
in Json format string.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getrawtransaction",
"params": ["0x2b64b0823f61a6be1a9b9fe2767a1e06b12a563a5f1d994b9adbc2387a907144", false],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "000050f1f011000001e72d286979ee6cb1b7e65dfddfb2e384100b8d148e7758de42e4168b71792c60400000000000000073ba0e94606a6d2ab49cac1411df5d1297c916da00"
}
```

