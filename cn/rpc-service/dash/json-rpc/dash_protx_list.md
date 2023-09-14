---
title: dash:protx_list \[POST\] {disallowed}
description: The protx list RPC returns a list of provider transactions.Lists all ProTxs in your wallet or on-chain, depending on the giventype.If type is not specified, it defaults to registered. All types have theoptional argument detailed which if set to true will result in adetailed list being returned. If set to false, only the hashes of theProTx will be returned.
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

