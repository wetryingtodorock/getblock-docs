---
title: geth:admin_startHTTP \[POST\] {disallowed}
description: The startHTTP administrative method starts an HTTP based JSON-RPC APIwebserver to handle client requests. All the parameters are optional.The method returns a boolean flag specifying whether the HTTP RPClistener was opened or not. Please note, only one HTTP endpoint isallowed to be active at any time.
---

### Parameters


`host` - string

network interface to open the listener socket on (defaults to
"localhost")

`port` - hexNumber

network port to open the listener socket on (defaults to 8545)

`cors` - string

cross-origin resource sharing header to use (defaults to "")

`apis` - string

API modules to offer over this interface (defaults to "eth,net,web3")

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_startHTTP",
"params": [],
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

