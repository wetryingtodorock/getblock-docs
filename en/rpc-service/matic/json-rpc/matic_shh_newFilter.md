---
title: matic:shh_newFilter \[POST\] {disallowed}
description: Creates filter to notify, when client receives whisper message matchingthe filter options.
---

### Parameters


`filters` - json object

filter object: { "to": "address" (string, optional) - Identity of the
receiver. When present it will try to decrypt any incoming message if
the client holds the private key to this identity. "topics": \["topic"\]
(array of string) - Array of topics which the incoming message’s topics
should match. }

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "shh_newFilter",
"params": [null],
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

