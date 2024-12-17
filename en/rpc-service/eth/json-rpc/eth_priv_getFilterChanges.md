---
title: eth:priv_getFilterChanges \[POST\] {disallowed}
description: Polls the specified filter for a private contract and returns an arrayof changes that have occurred since the last poll.Filters for private contracts can only be created by priv_newFilter sounlike eth_getFilterChanges, priv_getFilterChanges always returns anarray of log objects or an empty list.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`data` - None

Filter ID.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getFilterChanges",
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

