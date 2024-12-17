---
title: eth:perm_removeAccountsFromAllowlist \[POST\] {disallowed}
description: Removes accounts (participants) from the accounts permissions list.
---

### Parameters


`list of strings` - None

List of account addresses.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "perm_removeAccountsFromAllowlist",
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

