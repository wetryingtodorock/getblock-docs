---
title: kcc:eth_sign \[POST\] {disallowed}
description: The sign method calculates an Ethereum specific signature withsign(keccak256(\x19Ethereum Signed Message\n + len(message) +message))).By adding a prefix to the message makes the calculated signaturerecognisable as an Ethereum specific signature. This prevents misusewhere a malicious DApp can sign arbitrary data (e.g. transaction) anduse the signature to impersonate the victim.Note the address to sign with must be unlocked.
---

### Parameters


`DATA` - string

address.

`DATA` - string

message to sign.

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "0xdeadbeaf"],
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

