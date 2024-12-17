---
title: dash:getnewaddress \[POST\] {disallowed}
description: Returns a new Dash address for receiving payments. If label isspecified, the address is added to the address book so payments receivedwith the address will be associated with label.
---

### Parameters


`label` - string

Optional.

The label name for the address to be linked to. If not provided, the
default label "" is used. It can also be set to the empty string "" to
represent the default label.

The label does not need to exist, it will be created if there is no
label by the given name.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnewaddress",
"params": [null],
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

