---
title: dash:listtransactions \[POST\] {disallowed}
description: Returns the most recent transactions that affect the wallet. If a labelname is provided, this will return only incoming transactions paying toaddresses with the specified label.
---

### Parameters


`Label` - string

Optional.

If set, should be a valid label name to return only incoming
transactions with the specified label, or "\*" to disable filtering and
return all transactions.

`Count` - number (int)

Optional.

The number of the most recent transactions to list. Default is 10.

`Skip` - number (int)

Optional.

The number of the most recent transactions which should not be returned.
Allows for pagination of results. Default is 0.

`Include Watch-Only` - bool

Optional.

If set to true, include watch-only addresses in details and calculations
as if they were regular addresses belonging to the wallet.

If set to false (the default), treat watch-only addresses as if they
didn't belong to this wallet.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listtransactions",
"params": [null, null, null, null],
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

