---
title: avax:avax.getUTXOs \[WebSocket\] {disallowed}
description: Gets the UTXOs that reference a given address.
---

### Parameters


`addresses` - list

is a list of UTXOs such that each UTXO references at least one address
in addresses.

`limit` - int

Optional.

`startIndex` - map

Optional.

When using pagination (ie when startIndex is provided), UTXOs are not
guaranteed to be unique across multiple calls. That is, a UTXO may
appear in the result of the first call, and then again in the second
call.

When using pagination, consistency is not guaranteed across multiple
calls. That is, the UTXO set of the addresses may have changed between
calls.

Map format: {address: string; uxto: string}

`sourceChain` - string

source Chain

`encoding` - string

Optional.

encoding sets the format for the returned UTXOs. Can be either "cb58" or
"hex". Defaults to "cb58".

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.getUTXOs",
"params": [null, null, null, null, null],
"id": "getblock.io"}
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

