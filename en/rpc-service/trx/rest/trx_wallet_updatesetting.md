---
title: trx:/wallet/updatesetting \[POST\] {disallowed}
description: Update the consume_user_resource_percent parameter of a smart contract
---

### Parameters


`owner_address` - string, required

Transaction creator address, in hex string format.

`contract_address` - string, required

The address of the contract to be modified, in hex string format.

`consume_user_resource_percent` - int32, required

Consume user's resource percentage. It should be an integer between \[0,
100\]. if 0, means it does not consume user's resource until the
developer's resource has been used up

`permission_id` - int32

Optional. Whehter the address is in base58 format.

`visible` - boolean

Optional. Whehter the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/updatesetting' \
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

