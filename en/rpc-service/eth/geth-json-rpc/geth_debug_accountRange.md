---
title: geth:debug_accountRange \[POST\] {disallowed}
description: Enumerates all accounts at a given block with paging capability.maxResults are returned in the page and the items have keys that comeafter the start key (hashed address).If incompletes is false, then accounts for which the key preimage (i.ethe address) doesn’t exist in db are skipped. NB geth by default doesnot store preimages.
---

### Parameters


`blockNrOrHash` - string

block number or hash

`start` - string

start hashed address

`maxResults` - int

max results per page

`nocode` - bool

None

`nostorage` - bool

None

`incompletes` - bool

If incompletes is false, then accounts for which the key preimage (i.e:
the address) doesn’t exist in db are skipped.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_accountRange",
"params": ["123", "hashed.address", 5, true, true, true],
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

