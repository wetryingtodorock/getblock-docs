---
title: eth:priv_newFilter \[POST\] {disallowed}
description: Creates a log filter for a private contract. To poll for logs associatedwith the created filter, use priv_getFilterChanges. To get all logsassociated with the filter, use priv_getFilterLogs.For private contracts, priv_newFilter is the same as eth_newFilter forpublic contracts.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`Object` - None

Filter options object.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_newFilter",
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

