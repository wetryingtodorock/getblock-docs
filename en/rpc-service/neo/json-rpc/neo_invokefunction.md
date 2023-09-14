---
title: neo:invokefunction \[POST\] {disallowed}
description: Invokes a smart contract with its scripthash based on the specifiedoperation and parameters and returns the result.
---

### Parameters


`scripthash` - string

Smart contract scripthash. You need to use the proper byte order of the
address passed according to its data type. If the data type is Hash160,
use the big endian scripthash; if the data type is ByteArray, use the
little endian scripthash.

`operation` - string

The operation name

`params` - string

Optional. The parameters to be passed into the smart contract operation

`signers` - string

Optional. List of contract signature accounts.

\- account: signature account

\- scopes: signatures valid scopes, allowed values are:

\- None: Only transactions are signed and no contracts are allowed to
use this signature.

\- CalledByEntry: It only applies to the chain call entry. That is, if
the user invokes contract A, and then contract A calls contract B, only
contract A can use the signature. It is recommended as the default value
for the wallet.

\- CustomContracts: Custom contract. The signature can be used in the
specified contract. It can be used in conjunction with CalledByEntry.

\- CustomGroups: Custom contract groups that can be used in a specified
contract group. It can be used in conjunction with CalledByEntry.

\- Global: Global. Global. The risk is extremely high because the
contract may transfer all assets in the address. Only choose it when the
contract is extremely trusted.

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
"method": "invokefunction",
"params": [null, null, null, null],
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

