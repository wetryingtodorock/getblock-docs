---
title: bsv:lockunspent \[POST\] {disallowed}
description: Updates list of temporarily unspendable outputs.Temporarily lock (unlock=false) or unlock (unlock=true) specifiedtransaction outputs.If no transaction outputs are specified when unlocking then all currentlocked transaction outputs are unlocked.A locked transaction output will not be chosen by automatic coinselection, when spending bitcoins.Manually selected coins are automatically unlocked.Locks are stored in memory only. Nodes start with zero locked outputs,and the locked output list is always cleared (by virtue of process exit)when a node stops or fails.Also see the listunspent call
---

### Parameters


`unlock` - boolean, required

Whether to unlock (true) or lock (false) the specified transactions

`transactions` - json array, optional, default=empty array

The transaction outputs and within each, the txid (string) vout
(numeric).

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "lockunspent",
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

