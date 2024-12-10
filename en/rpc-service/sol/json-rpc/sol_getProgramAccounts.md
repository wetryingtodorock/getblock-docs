---
title: sol:getProgramAccounts - Solana
description: Example code for the sol:getProgramAccounts json-rpc method. Сomplete guide on how to use sol:getProgramAccounts json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Pubkey` - string

Pubkey of program, as base-58 encoded string

`Config` - object

Optional.

Configuration object containing the following optional fields: -
commitment (optional) - encoding: string (optional) - encoding for
Account data, either "base58" (slow), "base64", "base64+zstd", or
"jsonParsed". "base58" is limited to Account data of less than 129
bytes. "base64" will return base64 encoded data for Account data of any
size. "base64+zstd" compresses the Account data using Zstandard and
base64-encodes the result. "jsonParsed" encoding attempts to use
program-specific state parsers to return more human-readable and
explicit account state data. If "jsonParsed" is requested but a parser
cannot be found, the field falls back to "base64" encoding, detectable
when the data field is type string. - dataSlice: object (optional) -
limit the returned account data using the provided \[offset: usize\] and
\[length: usize\] fields; only available for "base58", "base64" or
"base64+zstd" encodings. - filters: array (optional) - filter results
using various filter objects; account must meet all filter criteria to
be included in results - withContext: bool (optional) - wrap the result
in an RpcResponse JSON object.

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getProgramAccounts",
"params": ["4Nd1mBQtrMJVYVfKf2PJy9NZUZdTAsp7D4xWLs4gDB4T", null],
"id": "getblock.io"}'
```

###  Response

``` java
null
```

