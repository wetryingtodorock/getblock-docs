---
title: geth:personal_sendTransaction \[POST\] {disallowed}
description: Validate the given passphrase and submit transaction.The transaction is the same argument as for eth_sendTransaction (i.e.transaction object) and contains the from address. If the passphrase canbe used to decrypt the private key belogging to tx.from the transactionis verified, signed and send onto the network. The account is notunlocked globally in the node and cannot be used in other RPC calls.
---

### Parameters


`tx` - json object

None

`passphrase` - string

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_sendTransaction",
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

