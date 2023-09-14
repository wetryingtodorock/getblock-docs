# bch:blockheaders \[GET\]

Given a block hash: returns amount of blockheaders in upward direction.
Returns empty if the block doesn't exist or it isn't in the active
chain.

### Example

`GET /rest/headers/<COUNT>/<BLOCK-HASH>.<bin|hex|json>`

### Request

``` java
curl --location --request GET 'https://bch.getblock.io/mainnet/rest/headers/10/00000000c937983704a73af28acdec37b049d214adbda81d7e2a3dd146f6ed09.json' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

### Response

``` java
[
    {
        "hash": "00000000c937983704a73af28acdec37b049d214adbda81d7e2a3dd146f6ed09",
        "confirmations": 679033,
        "height": 1000, 
        "version": 1, 
        "versionHex": "00000001",
        "merkleroot": "fe28050b93faea61fa88c4c630f0e1f0a1c24d0082dd0e10d369e13212128f33", 
        "time": 1232346882,
        "mediantime": 1232344831, 
        "nonce": 2595206198, 
        "bits": "1d00ffff", 
        "difficulty": 1,
        "chainwork": "000000000000000000000000000000000000000000000000000003e903e903e9", 
        "nTx": 1,
        "previousblockhash": "0000000008e647742775a230787d66fdf92c46a48c896bfbc85cdc8acc67e87d",
        "nextblockhash": "00000000a2887344f8db859e372e7e4bc26b23b9de340f725afbf2edb265b4c6"
    }
]
```
