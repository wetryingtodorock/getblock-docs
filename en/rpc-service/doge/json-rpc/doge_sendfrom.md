---
title: doge:sendfrom \[POST\] {disallowed}
description: Sends amount from account’s balance to dogecoinaddress.This method will fail if there is less than amount dogecoins withminconf confirmations in the account’s balance (unless account is theempty-string-named default account it behaves like the sendtoaddressmethod).Returns transaction ID on success.
---

### Parameters


`fromaccount` - string

Source account name.

`todogecoinaddress` - string

Dogecoin address to send to.

`amount` - float

Amount to send (float, rounded to the nearest 0.01).

`minconf` - integer

Minimum number of confirmations required for transferred balance.

`Comment` - string

Comment to add to transaction log.

`Comment_to` - string

Comment for to-address.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "sendfrom",
"params": [null, null, null, null, null, null],
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

