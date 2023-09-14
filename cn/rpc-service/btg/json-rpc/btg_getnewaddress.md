---
title: btg:getnewaddress \[POST\] {disallowed}
description: Returns a new Bitcoin address for receiving payments.If ‘label’ is specified, it is added to the address book so paymentsreceived with the address will be associated with ‘label’.
---

### Parameters


`label` - string, optional, default=””

The label name for the address to be linked to. It can also be set to
the empty string “” to represent the default label. The label does not
need to exist, it will be created if there is no label by the given
name.

`address_type` - string, optional, default=set by -addresstype

The address type to use. Options are “legacy”, “p2sh-segwit”, and
“bech32”.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnewaddress",
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

