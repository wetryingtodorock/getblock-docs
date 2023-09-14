---
title: geth:les_priorityClientInfo \[POST\] {disallowed}
description: Get individual client information on clients with a positive balance inthe specified ID range, start included, stop excluded. If stop is zerothen results are returned until the last existing balance entry.maxCount limits the number of returned results. If the count limit isreached but there are more IDs in the range then the first missing ID isincluded in the result with an empty value assigned to it.
---

### Parameters


`start` - id

start id, excluded

`stop` - id

stop id, included

`maxCount` - int

number of returned results.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "les_priorityClientInfo",
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

