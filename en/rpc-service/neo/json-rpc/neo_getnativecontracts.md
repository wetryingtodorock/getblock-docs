---
title: neo:getnativecontracts \[POST\]
description: Gets the native contracts list, which includes the basic information ofnative contracts and the contract descriptive file manifest.json.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnativecontracts",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        {
            "id": -1,
            "hash": "0xfffdc93764dbaddd97c48f252a53ea4643faa3fd",
            "nef": {
                "magic": 860243278,
                "compiler": "neo-core-v3.0",
                "tokens": [],
                "script": "EEEa93tnQBBBGvd7Z0AQQRr3e2dAEEEa93tnQBBBGvd7Z0AQQRr3e2dAEEEa93tnQBBBGvd7Z0A=",
                "checksum": 1110259869
            },
            "manifest": {
                "name": "ContractManagement",
                "groups": [],
                "supportedstandards": [],
                "abi": {
                    "methods": [
                        {
                            "name": "deploy",
                            "parameters": [
                                {
                                    "name": "nefFile",
                                    "type": "ByteArray"
                                },
                                {
                                    "name": "manifest",
                                    "type": "ByteArray"
                                }
                            ],
                            "returntype": "Array",
                            "offset": 0,
                            "safe": false
                        },
                        {
                            "name": "deploy",
                            "parameters": [
                                {
                                    "name": "nefFile",
                                    "type": "ByteArray"
                                },
                                {
                                    "name": "manifest",
                                    "type": "ByteArray"
                                },
                                {
                                    "name": "data",
                                    "type": "Any"
                                }
                            ],
                            "returntype": "Array",
                            "offset": 7,
                            "safe": false
                        },
                        {
                            "name": "destroy",
                            "parameters": [],
                            "returntype": "Void",
                            "offset": 14,
                            "safe": false
                        },
                        {
                            "name": "getContract",
                            "parameters": [
                                {
                                    "name": "hash",
                                    "type": "Hash160"
                                }
                            ],
                            "returntype": "Array",
                            "offset": 21,
                            "safe": true
                        },
                        {
                            "name": "getMinimumDeploymentFee",
                            "parameters": [],
                            "returntype": "Integer",
                            "offset": 28,
                            "safe": true
                        },
                        {
                            "name": "setMinimumDeploymentFee",
                            "parameters": [
                                {
                                    "name": "value",
                                    "type": "Integer"
                                }
                            ],
                            "returntype": "Void",
                            "offset": 35,
                            "safe": false
                        },
                        {
                            "name": "update",
                            "parameters": [
                                {
                                    "name": "nefFile",
                                    "type": "ByteArray"
                                },
                                {
                                    "name": "manifest",
                                    "type": "ByteArray"
                                }
                            ],
                            "returntype": "Void",
                            "offset": 42,
                            "safe": false
                        },
                        {
                            "name": "update",
                            "parameters": [
                                {
                                    "name": "nefFile",
                                    "type": "ByteArray"
                                },
                                {
                                    "name": "manifest",
                                    "type": "ByteArray"
                                },
                                {
                                    "name": "data",
                                    "type": "Any"
                                }
                            ],
                            "returntype": "Void",
                            "offset": 49,
                            "safe": false
                        }
                    ],
                    "events": [
                        {
                            "name": "Deploy",
                            "parameters": [
                                {
                                    "name": "Hash",
                                    "type": "Hash160"
                                }
                            ]
                        },
                        {
                            "name": "Update",
                            "parameters": [
                                {
                                    "name": "Hash",
                                    "type": "Hash160"
                                }
                            ]
                        },
                        {
                            "name": "Destroy",
                            "parameters": [
                                {
                                    "name": "Hash",
                                    "type": "Hash160"
                                }
                            ]
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
            },
            "updatehistory": [
                0
            ]
        }
    ]
}
```

