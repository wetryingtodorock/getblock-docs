---
title: ton:/getExtendedAddressInformation \[GET\]
description: Similar to \`/getAddressInformation\` but tries to parse additionalinformation for known contract types. This method is based on tonlibsfunction getAccountState. For detecting wallets we recommend to usegetWalletInformation.
---

### Parameters


`address` - query

required, string

Identifier of target TON account in any form.

### Request

``` java
curl --location --request GET 'https://ton.getblock.io/mainnet/getExtendedAddressInformation?address=EQAFPsHznqgqPUZQVyUBmWxpNwReAIuepKo_BjLiS-C05XB_' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "ok": true,
    "result": {
        "@extra": "1687338514.115839:6:0.5886804474003975",
        "@type": "fullAccountState",
        "account_state": {
            "@type": "wallet.v3.accountState",
            "seqno": 6,
            "wallet_id": "698983191"
        },
        "address": {
            "@type": "accountAddress",
            "account_address": "EQAFPsHznqgqPUZQVyUBmWxpNwReAIuepKo_BjLiS-C05XB_"
        },
        "balance": "809401535972",
        "block_id": {
            "@type": "ton.blockIdExt",
            "file_hash": "s6I65ivzwVkCLTCTVH0dIS7321rUFfx+4udx/9RRZB8=",
            "root_hash": "lV9RIaO7dQ01pfJhbzR5POMQ9uHgSqAAgcPpy4/K6qI=",
            "seqno": 30517690,
            "shard": "-9223372036854775808",
            "workchain": -1
        },
        "last_transaction_id": {
            "@type": "internal.transactionId",
            "hash": "R7vI2AxqgpQQYxQaxZsQwtZXHxE6rw6mDNtKJ3LtPVM=",
            "lt": "34789408000007"
        },
        "revision": 2,
        "sync_utime": 1687338490
    }
}
```

