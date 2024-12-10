---
title: sol:getAccountInfo - Solana
description: Example code for the sol:getAccountInfo json-rpc method. Сomplete guide on how to use sol:getAccountInfo json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Pubkey` - string

Pubkey of account to query, as base-58 encoded string

`Config` - object

Optional.

Configuration object containing the following optional fields: -
Commitment (optional) - encoding: string - encoding for Account data,
either "base58" (slow), "base64", "base64+zstd", or "jsonParsed".
"base58" is limited to Account data of less than 129 bytes. "base64"
will return base64 encoded data for Account data of any size.
"base64+zstd" compresses the Account data using Zstandard and
base64-encodes the result. "jsonParsed" encoding attempts to use
program-specific state parsers to return more human-readable and
explicit account state data. If "jsonParsed" is requested but a parser
cannot be found, the field falls back to "base64" encoding, detectable
when the data field is type string. - dataSlice: object (optional) -
limit the returned account data using the provided \[offset: usize\] and
\[length: usize\] fields; only available for "base58", "base64" or
"base64+zstd" encodings.

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getAccountInfo",
"params": ["vines1vzrYbzLMRdu58ou5XTby4qAqVRLmqo36NKPTg", [{"encoding": "base58"}]],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "jsonrpc": "2.0",
    "id": "getblock.io",
    "result": {
        "context": {
            "slot": 1
        },
        "value": {
            "data": [
                "11116bv5nS2h3y12kD1yUKeMZvGcKLSjQgX6BeV7u1FrjeJcKfsHRTPuR3oZ1EioKtYGiYxpxMG5vpbZLsbcBYBEmZZcMKaSoGx9JZeAuWf",
                "base58"
            ],
            "executable": false,
            "lamports": 1000000000,
            "owner": "11111111111111111111111111111111",
            "rentEpoch": 2
        }
    }
}
```

