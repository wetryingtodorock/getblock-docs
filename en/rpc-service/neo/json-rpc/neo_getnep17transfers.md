---
title: neo:getnep17transfers \[POST\] {disallowed}
description: Returns all the NEP17 transaction information occurred in the specifiedaddress.
---

### Parameters


`address` - string

The address to query the transaction information.

`startTime | endTime` - UTC timestamp, optional

The UTC timestamp which records the asset start or end time (included).

If start and end timestamps are specified, transactions occurred in the
time range are returned.

If only one timestamp is specified, transactions occurred since that
time are returned.

If not specified, transactions in recent seven days are returned.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnep17transfers",
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

