---
title: dash:protx_list  {disallowed} - Dash
description: Example code for the dash:protx_list  {disallowed} json-rpc method. Сomplete guide on how to use dash:protx_list  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`submethod` - string

None

`type` - string

Optional.

The type of ProTxs to list:

\- registered - all ProTxs registered at height

\- valid - all active/valid ProTxs at height

\- wallet - all ProTxs found in the current wallet

Height defaults to current chain-tip if one is not provided.

`detailed` - bool

Optional.

If set to false (default), only ProTx hashes are returned. If set to
true, a detailed list of ProTx details is returned.

`None` - None

Optional.

List ProTxs from this height (default: current chain tip).

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "protx",
"params": ["list", null, null, null],
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

