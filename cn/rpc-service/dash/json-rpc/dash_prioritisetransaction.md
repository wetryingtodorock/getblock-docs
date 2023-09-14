---
title: dash:prioritisetransaction \[POST\] {disallowed}
description: adds virtual priority or fee to a transaction, allowing it to beaccepted into blocks mined by this node (or miners which use this node)with a lower priority or fee.(It can also remove virtual priority or fee, requiring the transactionhave a higher priority or fee to be accepted into a locally-minedblock.)
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

