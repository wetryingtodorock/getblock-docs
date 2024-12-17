---
title: doge:sendfrom  {disallowed} - Dogecoin
description: Example code for the doge:sendfrom  {disallowed} json-rpc method. Сomplete guide on how to use doge:sendfrom  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

