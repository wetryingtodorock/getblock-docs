---
title: geth:personal_sign \[POST\] {disallowed}
description: The sign method calculates an Ethereum specific signature withsign(keccak256(\x19Ethereum Signed Message\n + len(message) +message)).By adding a prefix to the message makes the calculated signaturerecognisable as an Ethereum specific signature. This prevents misusewhere a malicious DApp can sign arbitrary data (e.g. transaction) anduse the signature to impersonate the victim.See ecRecover to verify the signature.
---

### Parameters


`message` - message

None

`account` - string

None

`passwords` - array of string

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_sign",
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

