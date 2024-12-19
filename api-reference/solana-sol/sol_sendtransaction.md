---
title: sendTransaction - Solana
description: Example code for the sendTransaction json-rpc method. Сomplete guide on how to use sendTransaction json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`transaction` - string

fully-signed Transaction, as encoded string

`config` - object

Configuration object containing the following field: - skipPreflight:
bool - if true, skip the preflight transaction checks (default: false) -
preflightCommitment: string (optional) - Commitment level to use for
preflight (default: "finalized"). - encoding: string (optional) -
Encoding used for the transaction data. Either "base58" (slow,
DEPRECATED), or "base64". (default: "base58"). - maxRetries: usize
(optional) - Maximum number of times for the RPC node to retry sending
the transaction to the leader. If this parameter not provided, the RPC
node will retry the transaction until it is finalized or until the
blockhash expires.

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "sendTransaction",
"params": ["4hXTCkRzt9WyecNzV1XPgCDfGAZzQKNxLXgynz5QDuWWPSAZBZSHptvWRL3BjCvzUXRdKvHL2b7yGrRQcWyaqsaBCncVG7BFggS8w9snUts67BSh3EqKpXLUm5UMHfD7ZBe9GhARjbNQMLJ1QD3Spr6oMTBU6EhdB4RD8CP2xUxr2u3d6fos36PD98XS6oX8TQjLpsMwncs5DAMiD4nNnR8NBfyghGCWvCVifVwvA8B8TJxE1aiyiv2L429BCWfyzAme5sZW8rDb14NeCQHhZbtNqfXhcp2tAnaAT", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32005,
        "data": {
            "numSlotsBehind": 90384
        },
        "message": "Node is behind by 90384 slots"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

