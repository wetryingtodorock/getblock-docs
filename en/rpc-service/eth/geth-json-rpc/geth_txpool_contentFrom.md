---
title: geth:txpool_contentFrom \[POST\]
description: Retrieves the transactions contained within the txpool, returningpending as well as queued transactions of this address, grouped bynonce.
---

### Parameters


`address` - string

txpool address

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "txpool_contentFrom",
"params": ["0x000db5cb74a30bbc2f21a3f3dd501e8e0585816a"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": {
        "pending": {
            "1": {
                "blockHash": null,
                "blockNumber": null,
                "from": "0x000db5cb74a30bbc2f21a3f3dd501e8e0585816a",
                "gas": "0x5208",
                "gasPrice": "0x1a13b8600",
                "hash": "0x6470a89b9e7f0665781360c369ab57c0c199df4cc32d973f2d4a7b34f084c3a4",
                "input": "0x",
                "nonce": "0x1",
                "to": "0x97a363e191f1f01459b2a9987edd7c01c962f4ce",
                "transactionIndex": null,
                "value": "0x19dd1f15f7000",
                "type": "0x0",
                "chainId": "0x1",
                "v": "0x25",
                "r": "0xd314b6ace6e4f48474de5c3b50f8507833ca590c7c9f50039d13fc7672284cae",
                "s": "0xe3962f0c7b342e3517a7a6e1a8c6ab51565840d93ca457caf462358ff2e612c"
            }
        },
        "queued": {}
    }
}
```

