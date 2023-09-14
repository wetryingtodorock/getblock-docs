# bch:blockhashbyheight \[GET\]

Given a height: returns hash of block in best-block-chain at height
provided.

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
