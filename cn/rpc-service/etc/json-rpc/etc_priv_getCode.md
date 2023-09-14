---
title: etc:priv_getCode \[POST\] {disallowed}
description: Returns the code of the private smart contract at the specified address.Compiled smart contract code is stored as a hexadecimal value.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`data` - None

20-byte contract address.

`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getCode",
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

