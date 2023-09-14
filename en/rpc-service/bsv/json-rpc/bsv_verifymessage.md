---
title: bsv:verifymessage \[POST\]
description: Verify a signed message
---

### Parameters


`address` - string, required

The btc address to use for the signature.

`signature` - string, required

The signature provided by the signer in base 64 encoding (see
signmessage).

`message` - string, required

The message that was signed.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "verifymessage",
"params": ["1D1ZrZNe3JUo7ZycKEYQQiQAWd9y54F4XX", "signature", "my message"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "isvalid": false
    }
}
```

