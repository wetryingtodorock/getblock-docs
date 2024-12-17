---
title: matic:eth_sign \[POST\]
description: The sign method calculates an Ethereum specific signature withsign(keccak256(\x19Ethereum Signed Message\n + len(message) +message))).By adding a prefix to the message makes the calculated signaturerecognisable as an Ethereum specific signature. This prevents misusewhere a malicious DApp can sign arbitrary data (e.g. transaction) anduse the signature to impersonate the victim.Note the address to sign with must be unlocked.
---

### Parameters


`DATA` - string

address.

`DATA` - string

message to sign.

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0xe7e2cb8c81c10ff191a73fe266788c9ce62ec754", "0xdeadbeaf"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "unknown account"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

