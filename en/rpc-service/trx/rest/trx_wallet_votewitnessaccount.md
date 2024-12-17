---
title: trx:/wallet/votewitnessaccount  {disallowed} - TRON
description: Example code for the trx:/wallet/votewitnessaccount  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/votewitnessaccount  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Owner address, default hexString

`votes` - array of json objects

format: - vote_address - string - stands for the address of the witness
you want to vote, default hexString, - vote_count - int_32 - stands for
the number of votes you want to vote

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/votewitnessaccount' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

