---
title: dash:quorum_list \[POST\] {disallowed}
description: displays a list of on-chain quorums.
---

### Parameters


`submethod` - string

None

`count` - nnumber

Optional.

Number of quorums to list. Will list active quorums if count is not
specified.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "quorum",
"params": ["list", null],
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

