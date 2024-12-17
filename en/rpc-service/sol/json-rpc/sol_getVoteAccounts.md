---
title: sol:getVoteAccounts - Solana
description: Example code for the sol:getVoteAccounts json-rpc method. Сomplete guide on how to use sol:getVoteAccounts json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`config` - object

Optional

Configuration object containing the following field: - commitment
(optional) - votePubkey: string (optional) - Only return results for
this validator vote address (base-58 encoded) - keepUnstakedDelinquents:
bool (optional) - Do not filter out delinquent validators with no
stake - delinquentSlotDistance: u64 (optional) - Specify the number of
slots behind the tip that a validator must fall to be considered
delinquent. NOTE: For the sake of consistency between ecosystem
products, it is not recommended that this argument be specified.

### Request

``` java
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "current": [
            {
                "activatedStake": 65136133648061,
                "commission": 10,
                "epochCredits": [
                    [
                        280,
                        3946620,
                        3579916
                    ],
                    [
                        281,
                        4303497,
                        3946620
                    ],
                    [
                        282,
                        4652270,
                        4303497
                    ],
                    [
                        283,
                        4999558,
                        4652270
                    ],
                    [
                        284,
                        5095638,
                        4999558
                    ]
                ],
                "epochVoteAccount": true,
                "lastVote": 122802577,
                "nodePubkey": "dpuDVLGSXT28Z3RGS28QBD5LUmcWARQVu36vXCEhhBg",
                "rootSlot": 122802546,
                "votePubkey": "6AqFc9V6PqyXJReuP12ATGggaVpG1Ppg4LFNvnqQYz8B"
            },
            {
                "activatedStake": 81872060716406,
                "commission": 10,
                "epochCredits": [
                    [
                        280,
                        7726424,
                        7359721
                    ],
                    [
                        281,
                        8083234,
                        7726424
                    ],
                    [
                        282,
                        8432165,
                        8083234
                    ],
                    [
                        283,
                        8779570,
                        8432165
                    ],
                    [
                        284,
                        8875323,
                        8779570
                    ]
                ],
                "epochVoteAccount": true,
                "lastVote": 122802575,
                "nodePubkey": "ECAq48skWmYJobngNd8ZDUQxB8y9KCaRAAzsfp3y2hjK",
                "rootSlot": 122802543,
                "votePubkey": "DcbnYSBPSscNZNUk39mj5xtjCUdXM6QA6oRa4KrnTdaC"
            }
        ]
    }
}
```

