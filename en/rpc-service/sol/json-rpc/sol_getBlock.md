---
title: getBlock - Solana
description: Example code for the getBlock json-rpc method. Сomplete guide on how to use getBlock json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`u64` - u64

slot, as u64 integer

`Config` - object

Optional.

Configuration object containing the following optional fields: -
encoding: string - encoding for Account data, either "base58" (slow),
"base64", "base64+zstd", or "jsonParsed". "base58" is limited to Account
data of less than 129 bytes. "base64" will return base64 encoded data
for Account data of any size. "base64+zstd" compresses the Account data
using Zstandard and base64-encodes the result. "jsonParsed" encoding
attempts to use program-specific state parsers to return more
human-readable and explicit account state data. If "jsonParsed" is
requested but a parser cannot be found, the field falls back to "base64"
encoding, detectable when the data field is type string. -
transaction.message.instructions: list If "jsonParsed" is requested but
a parser cannot be found, the instruction falls back to regular JSON
encoding (accounts, data, and programIdIndex fields). -
transactionDetails: string (optional) - level of transaction detail to
return, either "full", "signatures", or "none". If parameter not
provided, the default detail level is "full". - rewards: bool
(optional) - whether to populate the rewards array. If parameter not
provided, the default includes rewards. - Commitment (optional) -
"processed" is not supported. If parameter not provided, the default is
"finalized".

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBlock",
"params": [122788843, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHeight": 111018262,
        "blockTime": 1646009934,
        "blockhash": "Bmm7S3gKAbYLKqEWjFjoZ7PnDGB3C6vsJ1yjG6tznrCX",
        "parentSlot": 122788842,
        "previousBlockhash": "3XhDMjAQMcMJHgbb6aTG48MLCTHnDfwk7FHpJ4wN4ymj",
        "rewards": [
            {
                "commission": null,
                "lamports": -11967,
                "postBalance": 1464864,
                "pubkey": "52GwEMWZ5oTBF6qCNuE1Y5SNDheSjSyjARiFNEUbrsEL",
                "rewardType": "Rent"
            },
            {
                "commission": null,
                "lamports": 6722500,
                "postBalance": 4694146146,
                "pubkey": "DAHJgPKdmncYW8DmY6meaU953a7SktQ7eDGtWduC8W8m",
                "rewardType": "Fee"
            },
            {
                "commission": null,
                "lamports": 226,
                "postBalance": 915183364848,
                "pubkey": "EvnRmnMrd69kFdbLMxWkTn1icZ7DCceRhvmb2SJXqDo4",
                "rewardType": "Rent"
            }
        ],
        "transactions": [
            {
                "meta": {
                    "err": null,
                    "fee": 5000,
                    "innerInstructions": [],
                    "logMessages": [
                        "Program FsJ3A3u2vn5cTVofAjvy6y5kwABJAqYWpe4975bi2epH invoke [1]",
                        "Program FsJ3A3u2vn5cTVofAjvy6y5kwABJAqYWpe4975bi2epH consumed 32275 of 200000 compute units",
                        "Program FsJ3A3u2vn5cTVofAjvy6y5kwABJAqYWpe4975bi2epH success"
                    ],
                    "postBalances": [
                        28954045000,
                        23942400,
                        1169280,
                        1141440
                    ],
                    "postTokenBalances": [],
                    "preBalances": [
                        28954050000,
                        23942400,
                        1169280,
                        1141440
                    ],
                    "preTokenBalances": [],
                    "rewards": [],
                    "status": {
                        "Ok": null
                    }
                },
                "transaction": {
                    "message": {
                        "accountKeys": [
                            "5YXnWX6Mmd8hp7fCpAB3wQUrHt6WtjJrA5QjmBuySsDP",
                            "5ALDzwcRJfSyGdGyhP3kP628aqBNHZzLuVww7o9kdspe",
                            "SysvarC1ock11111111111111111111111111111111",
                            "FsJ3A3u2vn5cTVofAjvy6y5kwABJAqYWpe4975bi2epH"
                        ],
                        "header": {
                            "numReadonlySignedAccounts": 0,
                            "numReadonlyUnsignedAccounts": 2,
                            "numRequiredSignatures": 1
                        },
                        "instructions": [
                            {
                                "accounts": [
                                    0,
                                    1,
                                    2
                                ],
                                "data": "6mJFQAEssWECZ33ewGbTZAvtVaeV9QBGxMZvAabzAeqe7ffgxn9zbR",
                                "programIdIndex": 3
                            }
                        ],
                        "recentBlockhash": "FfnbGUXtfGHiZqnkSxC6pRZjGKfZqrdM4L2wPwgLCrcn"
                    },
                    "signatures": [
                        "2YBeDREvfocgiwmtwE7j2yNWj8vbSG3Uxw17HKYp2f2iNoBy3ps7MuTdQ31PPY5AmAEghgoKJbTGUn25m3SUY96c"
                    ]
                }
            }
        ]
    }
}
```

