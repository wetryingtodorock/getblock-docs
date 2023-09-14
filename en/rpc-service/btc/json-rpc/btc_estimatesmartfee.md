---
title: btc:estimatesmartfee \[POST\] {disallowed}
description: Estimates the approximate fee per kilobyte needed for a transaction tobegin confirmation within conf_target blocks if possible and return thenumber of blocks for which the estimate is valid. Uses virtualtransaction size as defined in BIP 141 (witness data is discounted).
---

### Parameters


`conf_target` - numeric, required

Confirmation target in blocks (1 - 1008)

`estimate_mode` - string, optional, default=CONSERVATIVE

The fee estimate mode.

Whether to return a more conservative estimate which also satisfies a
longer history.

A conservative estimate potentially returns a higher feerate and is more
likely to be sufficient for the desired target, but is not as responsive
to short term drops in the prevailing fee market.

Must be one of: UNSET, ECONOMICAL, CONSERVATIVE

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "estimatesmartfee",
"params": [1, "default"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": {
        "feerate": 0.00243871,
        "blocks": 2
    },
    "error": null,
    "id": "getblock.io"
}
```

