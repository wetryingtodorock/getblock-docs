---
title: neo:getwalletbalance \[POST\] {disallowed}
description: Returns the balance of the corresponding asset in the wallet, based onthe specified asset number.This method applies to the contract assets that conform to NEP-17standards.
---

### Parameters


`Asset_id` - string

Asset ID (asset identifier), which is the script hash of the contract
for contract assets.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getwalletbalance",
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

