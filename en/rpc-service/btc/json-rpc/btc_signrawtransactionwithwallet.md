---
title: btc:signrawtransactionwithwallet \[POST\] {disallowed}
description: Sign inputs for raw transaction (serialized, hex-encoded).The second optional argument (may be null) is an array of previoustransaction outputs that this transaction depends on but may not yet bein the block chain.Requires wallet passphrase to be set with walletpassphrase call ifwallet is encrypted.
---

### Parameters


`hexstring` - string, required

The transaction hex string

`prevtxs` - json array, optional

The previous dependent transaction outputs

`sighashtype` - string, optional, default=ALL

“ALL” “NONE” “SINGLE” “ALL\|ANYONECANPAY” “NONE\|ANYONECANPAY”
“SINGLE\|ANYONECANPAY”

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "signrawtransactionwithwallet",
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

