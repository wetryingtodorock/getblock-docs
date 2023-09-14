---
title: geth:clique_discard \[POST\] {disallowed}
description: This method drops a currently running proposal. The signer will not castfurther votes (either for or against) the address.
---

### Parameters


`address` - string

given address

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "clique_discard",
"params": ["0x000251Bd7762a21Df45175E6E571e83f68d15f3E"],
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

