---
title: sol:getLargestAccounts - Solana
description: Example code for the sol:getLargestAccounts json-rpc method. Сomplete guide on how to use sol:getLargestAccounts json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Config` - object

Optional.

Configuration object containing the following optional fields: -
commitment: object (optional) - filter: string (optional) - filter
results by account type; currently supported: circulating \|
nonCirculating

### Request

``` java
```

###  Response

``` java
{
    "jsonrpc": "2.0",
    "id": "getblock.io",
    "result": {
        "context": {
            "slot": 54
        },
        "value": [
            {
                "lamports": 999974,
                "address": "99P8ZgtJYe1buSK8JXkvpLh8xPsCFuLYhz9hQFNw93WJ"
            },
            {
                "lamports": 42,
                "address": "uPwWLo16MVehpyWqsLkK3Ka8nLowWvAHbBChqv2FZeL"
            },
            {
                "lamports": 42,
                "address": "aYJCgU7REfu3XF8b3QhkqgqQvLizx8zxuLBHA25PzDS"
            },
            {
                "lamports": 42,
                "address": "CTvHVtQ4gd4gUcw3bdVgZJJqApXE9nCbbbP4VTS5wE1D"
            },
            {
                "lamports": 20,
                "address": "4fq3xJ6kfrh9RkJQsmVd5gNMvJbuSHfErywvEjNQDPxu"
            },
            {
                "lamports": 4,
                "address": "AXJADheGVp9cruP8WYu46oNkRbeASngN5fPCMVGQqNHa"
            },
            {
                "lamports": 2,
                "address": "8NT8yS6LiwNprgW4yM1jPPow7CwRUotddBVkrkWgYp24"
            }
        ]
    }
}
```

