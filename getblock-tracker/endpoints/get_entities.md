---
title: get_entities \[GET\]
description: Get available entities and fields to create expression
---

- https://api.getblock.io/external/webhook/get_entities

## Request

### Headers

- **x-api-key** _string_ - GetBlock API key to access GetBlock Tracker API.

## Response

### Response successful [200]

Array of objects
- **entities** _array of objects_ - available entities.
- **operators** _array of objects_ - operators to types.

Object entity
- **fields** _array of objects_  - fields of entity.
- **name** _string_ - entity name.

Object field
- **type** _string_ - field type.
- **name** _string_ - field name.

Object operator
- **operators** _array of string_ - operators.
- **types** _array of string_ - the type from the field to which the operator can be applied.

### Response not successful [400, 500]

Object
- **description** _string_ - description of what went wrong.
- **status_code** _int_ - status code of the response.

### Examples

Request

```
curl --location --request GET 'https://api.getblock.io/external/webhook/get_entities' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

Response

```
{
    "entities": [
        {
            "name": "transaction",
            "fields": [
                {
                    "name": "blockHash",
                    "type": "hex_32"
                },
                {
                    "name": "blockNumber",
                    "type": "int"
                },
                {
                    "name": "from",
                    "type": "hex_20"
                },
                {
                    "name": "gas",
                    "type": "uint"
                },
                {
                    "name": "gasPrice",
                    "type": "int"
                },
                {
                    "name": "hash",
                    "type": "hex_32"
                },
                {
                    "name": "input",
                    "type": "hex_32"
                },
                {
                    "name": "nonce",
                    "type": "uint"
                },
                {
                    "name": "to",
                    "type": "hex_20"
                },
                {
                    "name": "transactionIndex",
                    "type": "uint"
                },
                {
                    "name": "value",
                    "type": "int"
                }
            ]
        },
        {
            "name": "receipt",
            "fields": [
                {
                    "name": "transactionHash",
                    "type": "hex_32"
                },
                {
                    "name": "transactionIndex",
                    "type": "uint"
                },
                {
                    "name": "blockHash",
                    "type": "hex_32"
                },
                {
                    "name": "blockNumber",
                    "type": "int"
                },
                {
                    "name": "from",
                    "type": "hex_20"
                },
                {
                    "name": "to",
                    "type": "hex_20"
                },
                {
                    "name": "cumulativeGasUsed",
                    "type": "int"
                },
                {
                    "name": "gasUsed",
                    "type": "int"
                },
                {
                    "name": "contractAddress",
                    "type": "hex_20"
                },
                {
                    "name": "root",
                    "type": "hex_32"
                },
                {
                    "name": "status",
                    "type": "int"
                }
            ]
        },
        {
            "name": "block",
            "fields": [
                {
                    "name": "number",
                    "type": "int"
                },
                {
                    "name": "hash",
                    "type": "hex_32"
                },
                {
                    "name": "parentHash",
                    "type": "hex_32"
                },
                {
                    "name": "nonce",
                    "type": "hex_8"
                },
                {
                    "name": "sha3Uncles",
                    "type": "hex_32"
                },
                {
                    "name": "transactionsRoot",
                    "type": "hex_32"
                },
                {
                    "name": "stateRoot",
                    "type": "hex_32"
                },
                {
                    "name": "receiptsRoot",
                    "type": "hex_32"
                },
                {
                    "name": "miner",
                    "type": "hex_20"
                },
                {
                    "name": "difficulty",
                    "type": "int"
                },
                {
                    "name": "totalDifficulty",
                    "type": "int"
                },
                {
                    "name": "extraData",
                    "type": "hex_32"
                },
                {
                    "name": "size",
                    "type": "uint"
                },
                {
                    "name": "gasLimit",
                    "type": "uint"
                },
                {
                    "name": "gasUsed",
                    "type": "uint"
                },
                {
                    "name": "timestamp",
                    "type": "timestamp"
                },
                {
                    "name": "transactions",
                    "type": "hex_32"
                },
                {
                    "name": "uncles",
                    "type": "hex_32"
                }
            ]
        }
    ],
    "operators": [
        {
            "types": [
                "int",
                "uint"
            ],
            "operators": [
                "==",
                "!=",
                "<",
                ">",
                "<=",
                ">="
            ]
        },
        {
            "types": [
                "hex_20",
                "hex_32"
            ],
            "operators": [
                "==",
                "!="
            ]
        },
        {
            "types": [
                "array"
            ],
            "operators": [
                "contain",
                "not contain"
            ]
        }
    ]
}
```
