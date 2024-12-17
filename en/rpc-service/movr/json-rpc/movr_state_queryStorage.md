---
title: movr:state_queryStorage \[POST\] {disallowed}
description: Query historical storage entries (by key) starting from a start block.
---

### Parameters


`keys` - Vector of StorageKey

list of storage keys

`fromBlock` - Hash

start block hash

`toBlock` - BlockHash

end block hash

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "state_queryStorage",
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

