---
title: trx:/wallet/deploycontract \[POST\] {disallowed}
description: Deploys a contract. Returns TransactionExtention, which contains anunsigned transaction.
---

### Parameters


`abi` - json

Smart Contract's Application Binary Interface

`bytecode` - string

The compiled contract's identifier, used to interact with the Virtual
Machine.

`fee_limit` - int32

Maximum TRX consumption, measured in SUN (1 TRX = 1,000,000 SUN).

`parameter` - string

Parameter passed to the constructor of the contract. Call the virtual
machine format of the parameter \[1, 2\], use the js tool provided by
remix, convert the parameter array \[1, 2\] called by the contract
caller into the parameter format required by the virtual machine.

`origin_energy_limit` - int32

The max energy which will be consumed by the owner in the process of
execution or creation of the contract, is an integer which should be
greater than 0.

`owner_address` - string

Contract owner address, converted to a hex string

`name` - string

Contract name

`call_value` - int32

Amount of TRX transferred with this transaction, measured in SUN (1TRX =
1,000,000 SUN)

`consume_user_resource_percent` - int32

The same as User Pay Ratio. The percentage of resources specified for
users who use this contract. This field accepts integers between \[0,
100\]. If it is 0, it means the user does not consume resources until
the developer resources are exhausted. However, it is strongly
recommended to set the value between 1 and 99 (inclusive). This is
prevent the contract developer from potential malicious infinite loop
time out attacks.

`permission_id` - int32

Optional. Whehter the address is in base58 format.

`visible` - boolean

Optional. Whehter the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/deploycontract' \
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

