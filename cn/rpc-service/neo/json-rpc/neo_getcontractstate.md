---
title: neo:getcontractstate \[POST\]
description: Queries the contract information with the contract script hash or nativecontract name.
---

### Parameters


`script_hash` - string

Contract script hash or the native contract name.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getcontractstate",
"params": ["0xef4073a0f2b305a38ec4050e4d3d28bc40ea63f5"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "id": -5,
        "updatecounter": 0,
        "hash": "0xef4073a0f2b305a38ec4050e4d3d28bc40ea63f5",
        "nef": {
            "magic": 860243278,
            "compiler": "neo-core-v3.0",
            "tokens": [],
            "script": "EEEa93tnQBBBGvd7Z0AQQRr3e2dAEEEa93tnQBBBGvd7Z0AQQRr3e2dAEEEa93tnQBBBGvd7Z0AQQRr3e2dAEEEa93tnQBBBGvd7Z0AQQRr3e2dAEEEa93tnQBBBGvd7Z0AQQRr3e2dAEEEa93tnQA==",
            "checksum": 1841570703
        },
        "manifest": {
            "name": "NeoToken",
            "groups": [],
            "supportedstandards": [
                "NEP-17"
            ],
            "abi": {
                "methods": [
                    {
                        "name": "balanceOf",
                        "parameters": [
                            {
                                "name": "account",
                                "type": "Hash160"
                            }
                        ],
                        "returntype": "Integer",
                        "offset": 0,
                        "safe": true
                    },
                    {
                        "name": "decimals",
                        "parameters": [],
                        "returntype": "Integer",
                        "offset": 7,
                        "safe": true
                    },
                    {
                        "name": "registerCandidate",
                        "parameters": [
                            {
                                "name": "pubkey",
                                "type": "PublicKey"
                            }
                        ],
                        "returntype": "Boolean",
                        "offset": 49,
                        "safe": false
                    }
                ]
            },
            "permissions": [
                {
                    "contract": "*",
                    "methods": "*"
                }
            ],
            "trusts": [],
            "extra": null
        }
    }
}
```

