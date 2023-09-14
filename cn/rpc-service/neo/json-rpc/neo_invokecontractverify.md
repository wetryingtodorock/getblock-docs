---
title: neo:invokecontractverify \[POST\] {disallowed}
description: Invokes the contract method Verify.Unlike the method invokefunction which executes the contract by theApplication trigger, invokecontractverify executes the contract by theVerification trigger and can pass parameters as params and signers.Specific parameter type and number depend on the smart contract toinvoke.This method is used to test your VM script as if they ran on theblockchain at that point in time. This RPC call does not affect theblockchain in any way.
---

### Parameters


`scripthash` - string

Smart contract scripthash.

`params` - string

The parameters to be passed to the smart contract operation. It must be
an empty array \[\] as by default Neo only accepts the verify function
without parameter.

`signers` - string

Optional. List of contract signature accounts.

\- account: signature account

\- scopes: signatures valid scopes, allowed values: FeeOnly,
CalledByEntry, CustomContracts, CustomGroups, Global

\- allowedcontracts: contracts of the signature can take effect, if
scopes is CustomContracts

\- allowedgroups: pubkeys of the signature can take effect, if scopes is
CustomGroups

You need to use the proper byte order of the address passed according to
its data type. If the data type is Hash160, use the big endian script
hash; if the data type is ByteArray, use the little endian scripthash.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "invokecontractverify",
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

