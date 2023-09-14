---
title: bsv:converttopsbt \[POST\]
description: Converts a network serialized transaction to a PSBT. This should be usedonly with createrawtransaction and fundrawtransaction createpsbt andwalletcreatefundedpsbt should be used for new applications.
---

### Parameters


`hexstring` - string, required

The hex string of a raw transaction

`permitsigdata` - boolean, optional, default=false

If true, any signatures in the input will be discarded and conversion
will continue. If false, RPC will fail if any signatures are present.

`iswitness` - boolean, optional, default=depends on heuristic tests

Whether the transaction hex is a serialized witness transaction.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "converttopsbt",
"params": ["rawtransaction", null, null],
"id": "getblock.io"}'
```

###  Response

``` java
null
```

