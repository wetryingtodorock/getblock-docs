---
title: sol:getConfirmedBlocks \[POST\] {disallowed}
description: DEPRECATED Please use getBlocks instead This method is expected to beremoved in solana-core v2.0Returns a list of confirmed blocks between two slots
---

### Parameters


`start_slot` - u64

start_slot, as u64 integer

`end_slot` - u64

Optional

end_slot, as u64 integer

`commitment` - string

Optional.

Commitment; "processed" is not supported. If parameter not provided, the
default is "finalized".

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getConfirmedBlocks",
"params": [null, null, null],
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

