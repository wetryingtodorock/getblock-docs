---
title: bch:signrawtransactionwithkey \[POST\]
description: Sign inputs for raw transaction (serialized, hex-encoded).The second argument is an array of base58-encoded private keys that willbe the only keys used to sign the transaction.The third optional argument (may be null) is an array of previoustransaction outputs that this transaction depends on but may not yet bein the block chain.
---

### Parameters


`hexstring` - string, required

The transaction hex string

`privkeys` - json array, required

The base58-encoded private keys for signing

`prevtxs` - json array, optional

The previous dependent transaction outputs

`sighashtype` - string, optional, default=ALL

The signature hash type. Must be one of:

ALL

NONE

SINGLE

ALL\|ANYONECANPAY

NONE\|ANYONECANPAY

SINGLE\|ANYONECANPAY

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "signrawtransactionwithkey",
"params": ["hexstring", "privkeys", null, null],
"id": "getblock.io"}'
```

###  Response

``` java
null
```

