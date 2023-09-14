---
title: geth:personal_signTransaction \[POST\] {disallowed}
description: SignTransaction will create a transaction from the given arguments andtries to sign it with the key associated with tx.from. If the givenpasswd isn’t able to decrypt the key it fails. The transaction isreturned in RLP-form, not broadcast to other nodes. The first argumentis a transaction object and the second argument is the password, similarto personal_sendTransaction.
---

### Parameters


`tx` - string

None

`passphrase` - string

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_signTransaction",
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

