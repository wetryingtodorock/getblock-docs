---
title: dash:verifyislock \[POST\] {disallowed}
description: Tests if a quorum signature is valid for an InstantSend Lock.
---

### Parameters


`id` - string (hex)

Signing request ID.

`txid` - string (hex)

The transaction id (TXID).

`signature` - string (hex)

The InstantSend Lock signature to verify.

`maxHeight` - number

Optional.

The maximum height to search quorums from.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "verifyislock",
"params": [null, null, null, null],
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

