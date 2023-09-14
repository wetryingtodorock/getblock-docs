---
title: btg:psbtbumpfee \[POST\] {disallowed}
description: Bumps the fee of an opt-in-RBF transaction T, replacing it with a newtransaction B.Returns a PSBT instead of creating and signing a new transaction.An opt-in RBF transaction with the given txid must be in the wallet.The command will pay the additional fee by reducing change outputs oradding inputs when necessary.It may add a new change output if one does not already exist.All inputs in the original transaction will be included in thereplacement transaction.The command will fail if the wallet or mempool contains a transactionthat spends one of T’s outputs.By default, the new fee will be calculated automatically using theestimatesmartfee RPC.The user can specify a confirmation target for estimatesmartfee.Alternatively, the user can specify a fee rate in sat/vB for the newtransaction.At a minimum, the new fee rate must be high enough to pay an additionalnew relay fee (incrementalfee returned by getnetworkinfo) to enter thenode’s mempool.
---

### Parameters


`txid` - string, required

The txid to be bumped

`options` - json object, optional

None

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "psbtbumpfee",
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

