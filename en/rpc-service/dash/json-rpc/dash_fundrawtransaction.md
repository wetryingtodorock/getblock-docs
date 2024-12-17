---
title: dash:fundrawtransaction \[POST\] {disallowed}
description: Requires wallet support (unavailable on masternodes).Adds inputs to a transaction until it has enough in value to meet itsout value. This will not modify existing inputs, and will add one changeoutput to the outputs.Note that inputs which were signed may need to be resigned aftercompletion since in/outputs have been added. The inputs added will notbe signed, use signrawtransaction for that.All existing inputs must have their previous output transaction be inthe wallet.
---

### Parameters


`Hex string` - string (hex)

The hex string of the raw transaction.

`Options` - object

Optional.

Additional options.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "fundrawtransaction",
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

