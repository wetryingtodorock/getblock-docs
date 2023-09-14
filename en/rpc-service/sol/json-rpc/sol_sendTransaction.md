---
title: sol:sendTransaction \[POST\]
description: Submits a signed transaction to the cluster for processing.This method does not alter the transaction in any way it relays thetransaction created by clients to the node as-is.If the nodes rpc service receives the transaction, this methodimmediately succeeds, without waiting for any confirmations. Asuccessful response from this method does not guarantee the transactionis processed or confirmed by the cluster.While the rpc service will reasonably retry to submit it, thetransaction could be rejected if transactions recent_blockhash expiresbefore it lands.Use getSignatureStatuses to ensure a transaction is processed andconfirmed.Before submitting, the following preflight checks are performed - Thetransaction signatures are verified - The transaction is simulatedagainst the bank slot specified by the preflight commitment. On failurean error will be returned. Preflight checks may be disabled if desired.It is recommended to specify the same commitment and preflightcommitment to avoid confusing behavior.The returned signature is the first signature in the transaction, whichis used to identify the transaction (transaction id). This identifiercan be easily extracted from the transaction data before submission.
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

