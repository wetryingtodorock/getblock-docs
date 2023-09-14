---
title: etc:txpool_besuPendingTransactions \[POST\] {disallowed}
description: Lists pending transactions that match the supplied filter conditions.
---

### Parameters


`numResults` - number

Integer representing the maximum number of results to return.

`fields` - object

Object of fields used to create the filter condition.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "txpool_besuPendingTransactions",
"params": [2, {"from": {"eq": "0xfe3b557e8fb62b89f4916b721be55ceb828dbd73"}, "gas": {"lt": "0x5209"}, "nonce": {"gt": "0x1"}}],
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

