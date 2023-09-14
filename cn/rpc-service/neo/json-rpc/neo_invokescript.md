---
title: neo:invokescript \[POST\] {disallowed}
description: Returns the result after passing a script through the VM.
---

### Parameters


`script` - string

A script runnable in the VM. This is the same script that is returned in
invokefunction

`signers` - string

list of contract signature accounts

account: signature account

scopes: signatures valid scopes, allowed values: FeeOnly, CalledByEntry,
CustomContracts, CustomGroups, Global

allowedcontracts: contracts of the signature can take effect, if scopes
is CustomContracts

allowedgroups: pubkeys of the signature can take effect, if scopes is
CustomGroups

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "invokescript",
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

