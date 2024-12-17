---
title: movr:state_getRuntimeVersion \[POST\]
description: Get the runtime version.
---

### Parameters


`at` - BlockHash

0x7e8691febbd7deeebcc48e4cdff335ce7c73c825b45661400fd9fea2fadee9b9

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "state_getRuntimeVersion",
"params": [null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "apis": [
            [
                "0xdf6acb689907609b",
                4
            ],
            [
                "0x37e397fc7c91f5e4",
                2
            ],
            [
                "0x40fe3ad401f8959a",
                6
            ]
        ],
        "authoringVersion": 0,
        "implName": "parity-polkadot",
        "implVersion": 0,
        "specName": "polkadot",
        "specVersion": 9420,
        "stateVersion": 0,
        "transactionVersion": 23
    }
}
```

