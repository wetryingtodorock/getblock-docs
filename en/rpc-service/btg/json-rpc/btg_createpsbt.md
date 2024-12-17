---
title: btg:createpsbt \[POST\]
description: Creates a transaction in the Partially Signed Transaction format.Implements the Creator role.
---

### Parameters


`inputs` - json array, required

A json array of json objects

`outputs` - json array, required

a json array with outputs (key-value pairs), where none of the keys are
duplicated.

`locktime` - numeric, optional, default=0

Raw locktime. Non-0 value also locktime-activates inputs

`replaceable` - boolean, optional, default=false

Marks this transaction as BIP125 replaceable.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "createpsbt",
"params": [[{"txid": "myid", "vout": 0}], [{"data": "00010203"}], null, null],
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

