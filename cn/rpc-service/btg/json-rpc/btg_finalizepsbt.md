---
title: btg:finalizepsbt \[POST\]
description: Finalize the inputs of a PSBT. If the transaction is fully signed, itwill produce a network serialized transaction which can be broadcastwith sendrawtransaction. Otherwise a PSBT will be created which has thefinal_scriptSig and final_scriptWitness fields filled for inputs thatare complete.Implements the Finalizer and Extractor roles.
---

### Parameters


`psbt` - string, required

A base64 string of a PSBT

`extract` - boolean, optional, default=true

If true and the transaction is complete, extract and return the complete
transaction in normal network serialization instead of the PSBT.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "finalizepsbt",
"params": ["psbt", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```

