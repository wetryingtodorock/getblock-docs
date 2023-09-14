---
title: sol:getMultipleAccounts \[POST\]
description: Returns the account information for a list of Pubkeys
---

### Parameters


`Pubkeys` - array

An array of Pubkeys to query, as base-58 encoded strings

`Config` - object

Optional.

Configuration object containing the following optional fields: -
commitment (optional) - encoding: string - encoding for Account data,
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
"method": "getMultipleAccounts",
"params": [[["vines1vzrYbzLMRdu58ou5XTby4qAqVRLmqo36NKPTg", "4fYNw3dojWmQ4dXtSGE9epjRGy9pFSx62YypT7avPYvA"]], [{"dataSlice": {"offset": 0, "lenght": 0}}]],
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
        "value": [
            {
                "data": [
                    "AAAAAAEAAAACtzNsyJrW0g==",
                    "base64"
                ],
                "executable": false,
                "lamports": 1000000000,
                "owner": "11111111111111111111111111111111",
                "rentEpoch": 2
            },
            {
                "data": [
                    "",
                    "base64"
                ],
                "executable": false,
                "lamports": 5000000000,
                "owner": "11111111111111111111111111111111",
                "rentEpoch": 2
            }
        ]
    }
}
```

