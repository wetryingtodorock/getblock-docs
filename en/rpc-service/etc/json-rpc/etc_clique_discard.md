---
title: etc:clique_discard \[POST\] {disallowed}
description: Discards a proposal to add or remove a signer with the specifiedaddress.
---

### Parameters


`data` - None

20-byte address of proposed signer.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "clique_discard",
"params": [null],
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

