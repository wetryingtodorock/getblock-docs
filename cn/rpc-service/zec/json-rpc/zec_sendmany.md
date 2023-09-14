---
title: zec:sendmany \[POST\] {disallowed}
description: Send multiple times. Amounts are decimal numbers with at most 8 digitsof precision.
---

### Parameters


`fromaccount` - string

MUST be set to the empty string "" to represent the default account.
Passing any other string will result in an error.

`amounts` - None

A json object with addresses and amounts

{ "address":amount (numeric) The Zcash address is the key, the numeric
amount in ZEC is the value ,... }

`minconf` - numeric

Optional, default=1

Only use the balance confirmed at least this many times.

`comment` - string

Optional

A comment.

`subtractfeefromamount` - string

Optional.

A json array with addresses.

The fee will be equally deducted from the amount of each selected
address.

Those recipients will receive less Zcash than you enter in their
corresponding amount field.

If no addresses are specified here, the sender pays the fee.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "sendmany",
"params": [null, null, null, null, null],
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

