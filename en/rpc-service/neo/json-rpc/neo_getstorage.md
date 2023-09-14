---
title: neo:getstorage \[POST\]
description: Returns the stored value according to the contract script hash and thestored key. Both key and value are Base64-encoded.
---

### Parameters


`script_hash` - string

Contract script hash or contract ID

`key` - string

The key to look up in storage (Base64-encoded)

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getstorage",
"params": ["0x99042d380f2b754175717bb932a911bc0bb0ad7d", "aGVsbG8="],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "d29ybGQ="
}
```

