---
title: eth:clique_propose \[POST\] {disallowed}
description: Propose to add or remove a signer with the specified address.
---

### Parameters


`data` - None

20-byte address.

`boolean` - None

true to propose adding signer or false to propose removing signer.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "clique_propose",
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

