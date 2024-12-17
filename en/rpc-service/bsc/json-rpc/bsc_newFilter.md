---
title: bsc:newFilter \[POST\] {disallowed}
description: Creates filter to notify, when client receives whisper message matchingthe filter options.
---

### Parameters


`to` - DATA

60 Bytes - (optional) Identity of the receiver. When present it will try
to decrypt any incoming message if the client holds the private key to
this identity.

`topics` - Array of DATA

Array of DATA topics which the incoming message's topics should match.

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "newFilter",
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

