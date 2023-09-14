---
title: doge:sendmany \[POST\] {disallowed}
description: Sends specified amounts from account’s balance to dogecoinaddresses.This method will fail if there is less than total amount dogecoins withminconf confirmations in the account’s balance (unless account is theempty-string-named default account).Returns transaction ID on success.
---

### Parameters


`fromaccount` - string

Account to send from.

`todict` - dict

Dictionary with Dogecoin addresses as keys and amounts as values.

`minconf` - integer

Minimum number of confirmations required for transferred balance.

`Comment` - string

Optional.

Comment for transaction.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "sendmany",
"params": [null, null, 1, null],
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

