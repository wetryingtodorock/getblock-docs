---
title: xlm:/ledgers/{sequence}/transactions \[GET\]
description: This endpoint represents successful transactions in a given ledger.
---

### Parameters


`sequence` - path

integer, optional

The sequence number of a specific ledger.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

string, optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument isn’t
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn’t designated, it defaults to 10.

`include_failed` - query

boolean, optional

Set to true to include failed operations in results. Options include
true and false.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/ledgers/45678721/transactions?limit=1' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_embedded": {
        "records": [
            {
                "_links": {
                    "account": {
                        "href": "https://xlm.getblock.io/accounts/GC3YHATVYTGUWTPCPJHZBUPT5DMITMTHAMQVBWQX4KWUABF4234VS4IU"
                    },
                    "effects": {
                        "href": "https://xlm.getblock.io/transactions/fe71caa5e0a215a6a809161afb15373596b65852a5c1002fc3c44244698e445b/effects{?cursor,limit,order}",
                        "templated": true
                    },
                    "ledger": {
                        "href": "https://xlm.getblock.io/ledgers/45678721"
                    },
                    "operations": {
                        "href": "https://xlm.getblock.io/transactions/fe71caa5e0a215a6a809161afb15373596b65852a5c1002fc3c44244698e445b/operations{?cursor,limit,order}",
                        "templated": true
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/transactions?order=asc&cursor=196188612818116608"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/transactions/fe71caa5e0a215a6a809161afb15373596b65852a5c1002fc3c44244698e445b"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/transactions?order=desc&cursor=196188612818116608"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/fe71caa5e0a215a6a809161afb15373596b65852a5c1002fc3c44244698e445b"
                    }
                },
                "created_at": "2023-04-04T10:14:56Z",
                "envelope_xdr": "AAAAAgAAAAC3g4J1xM1LTeJ6T5DR8+jYibJnAyFQ2hfirUAEvNb5WQAAE4gCgsCJAANLsAAAAAEAAAAAAAAAAAAAAABkK/i2AAAAAAAAAAEAAAAAAAAADAAAAAJlV0hJUAAAAAAAAAAAAAAAWUh3GRDH8nbI8LdKFAI69RD/GVI2XpRSrp+mI0tjS18AAAAAAAAAACF501o23qgFAH+I5AAAAABJT2LoAAAAAAAAAAG81vlZAAAAQK6uLyjdCY1M4sAjarRPcvJftl6iqD21fj0cYtyUJPH2TpfQeJURhCniy5Erp2SiaMZu7eF6/GiYZB15cHV7iwk=",
                "fee_account": "GC3YHATVYTGUWTPCPJHZBUPT5DMITMTHAMQVBWQX4KWUABF4234VS4IU",
                "fee_charged": "100",
                "fee_meta_xdr": "AAAAAgAAAAMCuQBqAAAAAAAAAAC3g4J1xM1LTeJ6T5DR8+jYibJnAyFQ2hfirUAEvNb5WQAAAA/L2tXBAoLAiQADS68AAAAEAAAAAAAAAAAAAAAAAQAAAAAAAAAAAAABAAAAAEMF0YEAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAADAAAAAAK5AGoAAAAAZCv4HQAAAAAAAAABArkAgQAAAAAAAAAAt4OCdcTNS03iek+Q0fPo2ImyZwMhUNoX4q1ABLzW+VkAAAAPy9rVXQKCwIkAA0uvAAAABAAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAQAAAABDBdGBAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuQBqAAAAAGQr+B0AAAAA",
                "hash": "fe71caa5e0a215a6a809161afb15373596b65852a5c1002fc3c44244698e445b",
                "id": "fe71caa5e0a215a6a809161afb15373596b65852a5c1002fc3c44244698e445b",
                "ledger": 45678721,
                "max_fee": "5000",
                "memo_type": "none",
                "operation_count": 1,
                "paging_token": "196188612818116608",
                "preconditions": {
                    "timebounds": {
                        "max_time": "1680603318",
                        "min_time": "0"
                    }
                },
                "result_meta_xdr": "AAAAAgAAAAIAAAADArkAgQAAAAAAAAAAt4OCdcTNS03iek+Q0fPo2ImyZwMhUNoX4q1ABLzW+VkAAAAPy9rVXQKCwIkAA0uvAAAABAAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAQAAAABDBdGBAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuQBqAAAAAGQr+B0AAAAAAAAAAQK5AIEAAAAAAAAAALeDgnXEzUtN4npPkNHz6NiJsmcDIVDaF+KtQAS81vlZAAAAD8va1V0CgsCJAANLsAAAAAQAAAAAAAAAAAAAAAABAAAAAAAAAAAAAAEAAAAAQwXRgQAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAMAAAAAArkAgQAAAABkK/igAAAAAAAAAAEAAAAGAAAAAwK5AGoAAAACAAAAALeDgnXEzUtN4npPkNHz6NiJsmcDIVDaF+KtQAS81vlZAAAAAElPYugAAAACZVdISVAAAAAAAAAAAAAAAFlIdxkQx/J2yPC3ShQCOvUQ/xlSNl6UUq6fpiNLY0tfAAAAAAAAAA5nB1jwACkFDxGl5oAAAAAAAAAAAAAAAAAAAAABArkAgQAAAAIAAAAAt4OCdcTNS03iek+Q0fPo2ImyZwMhUNoX4q1ABLzW+VkAAAAASU9i6AAAAAJlV0hJUAAAAAAAAAAAAAAAWUh3GRDH8nbI8LdKFAI69RD/GVI2XpRSrp+mI0tjS18AAAAAAAAADmcHVRcAf4jkNt6oBQAAAAAAAAAAAAAAAAAAAAMCuQCBAAAAAAAAAAC3g4J1xM1LTeJ6T5DR8+jYibJnAyFQ2hfirUAEvNb5WQAAAA/L2tVdAoLAiQADS7AAAAAEAAAAAAAAAAAAAAAAAQAAAAAAAAAAAAABAAAAAEMF0YEAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAADAAAAAAK5AIEAAAAAZCv4oAAAAAAAAAABArkAgQAAAAAAAAAAt4OCdcTNS03iek+Q0fPo2ImyZwMhUNoX4q1ABLzW+VkAAAAPy9rVXQKCwIkAA0uwAAAABAAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAQAAAABDBcyhAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuQCBAAAAAGQr+KAAAAAAAAAAAwK5AGoAAAABAAAAALeDgnXEzUtN4npPkNHz6NiJsmcDIVDaF+KtQAS81vlZAAAAAmVXSElQAAAAAAAAAAAAAABZSHcZEMfydsjwt0oUAjr1EP8ZUjZelFKun6YjS2NLXwAAAB0kJnP1f/////////8AAAABAAAAAQAAAAAAAAAAAAAAHNFL/hkAAAAAAAAAAAAAAAECuQCBAAAAAQAAAAC3g4J1xM1LTeJ6T5DR8+jYibJnAyFQ2hfirUAEvNb5WQAAAAJlV0hJUAAAAAAAAAAAAAAAWUh3GRDH8nbI8LdKFAI69RD/GVI2XpRSrp+mI0tjS18AAAAdJCZz9X//////////AAAAAQAAAAEAAAAAAAAAAAAAABzRS/pAAAAAAAAAAAAAAAAA",
                "result_xdr": "AAAAAAAAAGQAAAAAAAAAAQAAAAAAAAAMAAAAAAAAAAAAAAABAAAAALeDgnXEzUtN4npPkNHz6NiJsmcDIVDaF+KtQAS81vlZAAAAAElPYugAAAACZVdISVAAAAAAAAAAAAAAAFlIdxkQx/J2yPC3ShQCOvUQ/xlSNl6UUq6fpiNLY0tfAAAAAAAAAA5nB1UXAH+I5DbeqAUAAAAAAAAAAAAAAAA=",
                "signatures": [
                    "rq4vKN0JjUziwCNqtE9y8l+2XqKoPbV+PRxi3JQk8fZOl9B4lRGEKeLLkSunZKJoxm7t4Xr8aJhkHXlwdXuLCQ=="
                ],
                "source_account": "GC3YHATVYTGUWTPCPJHZBUPT5DMITMTHAMQVBWQX4KWUABF4234VS4IU",
                "source_account_sequence": "180918629691509680",
                "successful": true,
                "valid_after": "1970-01-01T00:00:00Z",
                "valid_before": "2023-04-04T10:15:18Z"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/ledgers/45678721/transactions?cursor=196188612818116608&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/ledgers/45678721/transactions?cursor=196188612818112512&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/ledgers/45678721/transactions?cursor=&limit=2&order=asc"
        }
    }
}
```

