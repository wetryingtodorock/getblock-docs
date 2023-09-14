---
title: dgb:signmessage \[POST\] {disallowed}
description: Sign a message with the private key of an address Requires walletpassphrase to be set with walletpassphrase call if wallet is encrypted.
---

### Parameters


`address` - string, required

The bitcoin address to use for the private key.

`message` - string, required

The message to create a signature of.

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "signmessage",
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

