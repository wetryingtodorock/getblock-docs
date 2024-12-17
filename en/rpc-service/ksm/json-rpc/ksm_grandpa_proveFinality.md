---
title: ksm:grandpa_proveFinality \[POST\] {disallowed}
description: Prove finality for the range (begin end\] hash.
---

### Parameters


`begin` - BlockHash

start block hash

`end` - BlockHash

end block hash

`authoritiesSetId` - u64

set id

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "grandpa_proveFinality",
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

