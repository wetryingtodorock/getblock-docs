---
title: btc:blockhashbyheight - Bitcoin
description: Example code for the btc:blockhashbyheight rest method. Сomplete guide on how to use btc:blockhashbyheight rest in GetBlock.io Web3 documentation.
---

### Example

`GET /rest/blockhashbyheight/<HEIGHT>.<bin|hex|json>`

### Request

``` java
curl --location --request GET 'https://btc.getblock.io/rest/blockhashbyheight/10.json' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

### Response

``` java
{
    "blockhash":"000000002c05cc2e78923c34df87fd108b22221ac6076c18f3ade378a4d915e9"
}
```
