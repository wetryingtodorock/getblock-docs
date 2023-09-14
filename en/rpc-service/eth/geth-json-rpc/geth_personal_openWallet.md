---
title: geth:personal_openWallet \[POST\] {disallowed}
description: Initiates a hardware wallet opening procedure by establishing a USBconnection and then attempting to authenticate via the providedpassphrase. Note, the method may return an extra challenge requiring asecond open (e.g. the Trezor PIN matrix challenge).
---

### Parameters


`url` - string

None

`passphrase` - string

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_openWallet",
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

