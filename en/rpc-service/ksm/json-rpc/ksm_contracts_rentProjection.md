---
title: ksm:contracts_rentProjection \[POST\] {disallowed}
description: Returns the projected time a given contract will be able to sustainpaying its rent.
---

### Parameters


`address` - AccountId

None

`at` - BlockHash

None

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "contracts_rentProjection",
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

