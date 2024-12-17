---
title: sol:simulateTransaction - Solana
description: Example code for the sol:simulateTransaction json-rpc method. Сomplete guide on how to use sol:simulateTransaction json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`transaction` - string

Transaction, as an encoded string. The transaction must have a valid
blockhash, but is not required to be signed.

`Config` - object

Optional.

Configuration object containing the following fields: - sigVerify:
bool - if true the transaction signatures will be verified (default:
false, conflicts with replaceRecentBlockhash) - commitment: string
(optional) - Commitment level to simulate the transaction at (default:
"finalized"). - encoding: string (optional) - Encoding used for the
transaction data. Either "base58" (slow, DEPRECATED), or "base64".
(default: "base58"). - replaceRecentBlockhash: bool (optional) - if true
the transaction recent blockhash will be replaced with the most recent
blockhash. (default: false, conflicts with sigVerify) - accounts: object
(optional) - Accounts configuration object containing the following
fields: - encoding: string (optional) - encoding for returned Account
data, either "base64" (default), "base64+zstd" or "jsonParsed".
"jsonParsed" encoding attempts to use program-specific state parsers to
return more human-readable and explicit account state data. If
"jsonParsed" is requested but a parser cannot be found, the field falls
back to binary encoding, detectable when the data field is type
string. - addresses: array - an array of accounts to return, as base-58
encoded strings

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "simulateTransaction",
"params": ["4hXTCkRzt9WyecNzV1XPgCDfGAZzQKNxLXgynz5QDuWWPSAZBZSHptvWRL3BjCvzUXRdKvHL2b7yGrRQcWyaqsaBCncVG7BFggS8w9snUts67BSh3EqKpXLUm5UMHfD7ZBe9GhARjbNQMLJ1QD3Spr6oMTBU6EhdB4RD8CP2xUxr2u3d6fos36PD98XS6oX8TQjLpsMwncs5DAMiD4nNnR8NBfyghGCWvCVifVwvA8B8TJxE1aiyiv2L429BCWfyzAme5sZW8rDb14NeCQHhZbtNqfXhcp2tAnaAT", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "context": {
            "slot": 123032941
        },
        "value": {
            "accounts": null,
            "err": "BlockhashNotFound",
            "logs": []
        }
    }
}
```

