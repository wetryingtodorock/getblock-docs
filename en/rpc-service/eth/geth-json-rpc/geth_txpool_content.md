---
title: geth:txpool_content \[POST\]
description: The content inspection property can be queried to list the exact detailsof all the transactions currently pending for inclusion in the nextblock(s), as well as the ones that are being scheduled for futureexecution only.The result is an object with two fields pending and queued. Each ofthese fields are associative arrays, in which each entry maps anorigin-address to a batch of scheduled transactions. These batchesthemselves are maps associating nonces with actual transactions.Please note, there may be multiple transactions associated with the sameaccount and nonce. This can happen if the user broadcast mutliple oneswith varying gas allowances (or even completely different transactions).
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "txpool_content",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "pending": {
            "0x000251Bd7762a21Df45175E6E571e83f68d15f3E": {
                "1": {
                    "blockHash": null,
                    "blockNumber": null,
                    "chainId": "0x1",
                    "from": "0x000251bd7762a21df45175e6e571e83f68d15f3e",
                    "gas": "0x5208",
                    "gasPrice": "0x1a13b8600",
                    "hash": "0xfbaa33ae8b5a12bce04320f9fd609e30a300331c3d67b5ba47b8d9ee21a9896c",
                    "input": "0x",
                    "nonce": "0x1",
                    "r": "0xd037ec2f976a58372dbad0dd8eeb6ec7d65a0578620ed6ddab010627d4215200",
                    "s": "0x7a6ae8f8ac910fbde59bb3485d24e84c88311083c633493dad990ad7311d6f73",
                    "to": "0x63a0e8e7c9e86cf58e188b98f55cedee42c3c902",
                    "transactionIndex": null,
                    "type": "0x0",
                    "v": "0x26",
                    "value": "0x19dd1f15f7000"
                }
            },
            "0x0003BE8bd8dBa04Ac4dE888A9ea02AcF73b61700": {
                "1": {
                    "blockHash": null,
                    "blockNumber": null,
                    "chainId": "0x1",
                    "from": "0x0003be8bd8dba04ac4de888a9ea02acf73b61700",
                    "gas": "0x5208",
                    "gasPrice": "0x1a13b8600",
                    "hash": "0x263cdd926f7a8e72a3c3186f093200b3a39b7376e3ef845f66a3672e931ded3d",
                    "input": "0x",
                    "nonce": "0x1",
                    "r": "0x9d51d7501cbb009f00e8871f26c829d3c658b83c5bf5644347f52a78d4d0b6ee",
                    "s": "0x69bea9e077502afe4b07eda84254a448ece323a8777567bb7cde26b3e279525c",
                    "to": "0xcf2f6fb91ae5d2a7c7d736c8f89ae51a8a3f57d2",
                    "transactionIndex": null,
                    "type": "0x0",
                    "v": "0x25",
                    "value": "0x19dd1f15f7000"
                }
            },
            "0x000DB5cb74A30bbc2F21A3F3DD501E8E0585816a": {
                "1": {
                    "blockHash": null,
                    "blockNumber": null,
                    "chainId": "0x1",
                    "from": "0x000db5cb74a30bbc2f21a3f3dd501e8e0585816a",
                    "gas": "0x5208",
                    "gasPrice": "0x1a13b8600",
                    "hash": "0x6470a89b9e7f0665781360c369ab57c0c199df4cc32d973f2d4a7b34f084c3a4",
                    "input": "0x",
                    "nonce": "0x1",
                    "r": "0xd314b6ace6e4f48474de5c3b50f8507833ca590c7c9f50039d13fc7672284cae",
                    "s": "0xe3962f0c7b342e3517a7a6e1a8c6ab51565840d93ca457caf462358ff2e612c",
                    "to": "0x97a363e191f1f01459b2a9987edd7c01c962f4ce",
                    "transactionIndex": null,
                    "type": "0x0",
                    "v": "0x25",
                    "value": "0x19dd1f15f7000"
                }
            }
        }
    }
}
```

