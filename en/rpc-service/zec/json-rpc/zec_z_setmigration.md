---
title: zec:z_setmigration \[POST\] {disallowed}
description: When enabled the Sprout to Sapling migration will attempt to migrate allfunds from this wallet’s Sprout addresses to either the address forSapling account 0 or the address specified by the parameter-migrationdestaddress.This migration is designed to minimize information leakage. As a resultfor wallets with a significant Sprout balance, this process may takeseveral weeks. The migration works by sending, up to 5, as manytransactions as possible whenever the blockchain reaches a height equalto 499 modulo 500. The transaction amounts are picked according to therandom distribution specified in ZIP 308. The migration will end oncethe wallet’s Sprout balance is below 0.01 ZEC.
---

### Parameters


`enabled` - boolean

"true" or "false" to enable of disable respectively.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_setmigration",
"params": [null],
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

