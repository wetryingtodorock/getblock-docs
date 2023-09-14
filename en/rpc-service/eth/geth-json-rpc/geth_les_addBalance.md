---
title: geth:les_addBalance \[POST\] {disallowed}
description: Add signed value to the token balance of the specified client and updateits meta tag. The balance cannot go below zero or over 2^^63-1. Thebalance values before and after the update are returned. The meta tagcan be used to store a sequence number or reference to the lastprocessed incoming payment, token expiration info, balance in othercurrencies or any application-specific additional information.
---

### Parameters


`id` - number

None

`value` - int64

None

`meta` - string

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "les_addBalance",
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

