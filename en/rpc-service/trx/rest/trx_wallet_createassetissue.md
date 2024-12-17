---
title: /wallet/createassetissue  {disallowed} - TRON
description: Example code for the /wallet/createassetissue  {disallowed} rest method. Сomplete guide on how to use /wallet/createassetissue  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Owner address, default hexString

`name` - string

Token name, default hexString

`abbr` - string

`total_supply` - int64

Token total supply

`trx_num` - int64

Define the price by the ratio of trx_num/num(The unit of 'trx_num' is
SUN)

`num` - int64

Define the price by the ratio of trx_num/num

`start_time` - date-time

ICO start time

`end_time` - date-time

ICO end time

`description` - string

Token description, default hexString

`url` - string

Token official website url, default hexString

`free_asset_net_limit` - int64

Token free asset net limit

`public_free_asset_net_limit` - int64

Token public free asset net limit

`frozen_supply` - json object

Token frozen supply

`precision` - int32

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createassetissue' \
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

