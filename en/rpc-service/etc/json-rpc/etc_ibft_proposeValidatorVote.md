---
title: etc:ibft_proposeValidatorVote \[POST\] {disallowed}
description: Propose to add or remove a validator with the specified address.
---

### Parameters


`data` - None

Account address

`boolean` - None

true to propose adding validator or false to propose removing validator.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "ibft_proposeValidatorVote",
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

