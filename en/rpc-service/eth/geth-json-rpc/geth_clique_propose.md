---
title: geth:clique_propose \[POST\] {disallowed}
description: Adds a new authorization proposal that the signer will attempt to pushthrough. If the auth parameter is false, the local signer votes for thegiven address to be included in the set of authorized signers. With authset to false, the vote is against the address.
---

### Parameters


`address` - string

address

`auth` - boolean

whether to vote for the given address or against it.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "clique_propose",
"params": ["0x000251Bd7762a21Df45175E6E571e83f68d15f3E", false],
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

