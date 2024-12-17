---
title: dash:prioritisetransaction  {disallowed} - Dash
description: Example code for the dash:prioritisetransaction  {disallowed} json-rpc method. Сomplete guide on how to use dash:prioritisetransaction  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`TXID` - string

The TXID of the transaction whose virtual priority or fee you want to
modify, encoded as hex in RPC byte order.

`fee` - number (int)

Warning: this value is in duffs, not Dash

If positive, the virtual fee to add to the actual fee paid by the
transaction; if negative, the virtual fee to subtract from the actual
fee paid by the transaction.

No change is made to the actual fee paid by the transaction.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "prioritisetransaction",
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

