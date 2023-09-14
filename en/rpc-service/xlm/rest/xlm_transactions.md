---
title: xlm:/transactions \[GET\]
description: This endpoint lists all Successful transactions and can be used instreaming mode. Streaming mode allows you to listen for new transactionsas they are added to the Stellar ledger. If called in streaming mode,Horizon will start at the earliest known transaction unless a cursor isset, in which case it will start from that cursor. By setting the cursorvalue to now, you can stream transactions created since your requesttime.
---

### Parameters


`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

string, optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument isn't
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn't designated, it defaults to 10.

`include_fail` - query

boolean, optional

Set to true to include failed operations in results. Options include
true and false.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/transactions?limit=1' 
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
                        "href": "https://xlm.getblock.io/accounts/GBUO63ZYZUGNJ6Z3OG2WQAYGVOPUD72REX6FKSAN3YOMUR3OYAPVYOPU"
                    },
                    "effects": {
                        "href": "https://xlm.getblock.io/transactions/f23e07e9b88ffdb04940fb8dfd625eb32dc19781896a101063f1a0975fc009f4/effects{?cursor,limit,order}",
                        "templated": true
                    },
                    "ledger": {
                        "href": "https://xlm.getblock.io/ledgers/45678720"
                    },
                    "operations": {
                        "href": "https://xlm.getblock.io/transactions/f23e07e9b88ffdb04940fb8dfd625eb32dc19781896a101063f1a0975fc009f4/operations{?cursor,limit,order}",
                        "templated": true
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/transactions?order=asc&cursor=196188608523149312"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/transactions/f23e07e9b88ffdb04940fb8dfd625eb32dc19781896a101063f1a0975fc009f4"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/transactions?order=desc&cursor=196188608523149312"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/f23e07e9b88ffdb04940fb8dfd625eb32dc19781896a101063f1a0975fc009f4"
                    }
                },
                "created_at": "2023-04-04T10:14:50Z",
                "envelope_xdr": "AAAAAgAAAABo7284zQzU+ztxtWgDBqufQf9RJfxVSA3eHMpHbsAfXAAAJxACkv50AAxlnQAAAAEAAAAAAAAAAAAAAABkK/i0AAAAAAAAAAEAAAAAAAAADAAAAAFVU0RWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAAAUdCUFYAAAAAw+y5PPMHIkazPoP3+FxZAWpug05W+hSRi4g6//ynAQQAAAABVPBGAAAAE5EAAA+gAAAAAAAAAAAAAAAAAAAAAW7AH1wAAABAAmwMLx7/HGzh95khPvaOr+sq9PuEyliGBi8ur7IKJ5QBjY3bImynfmh4nkqYaNcl9NmsbRYOkqISOlCbGJWYCA==",
                "fee_account": "GBUO63ZYZUGNJ6Z3OG2WQAYGVOPUD72REX6FKSAN3YOMUR3OYAPVYOPU",
                "fee_charged": "10000",
                "fee_meta_xdr": "AAAAAgAAAAMCuQB+AAAAAAAAAABo7284zQzU+ztxtWgDBqufQf9RJfxVSA3eHMpHbsAfXAAAAAADPpT+ApL+dAAMZZwAAAAHAAAAAAAAAAAAAAAAAQAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAADAAAAAAK5AH4AAAAAZCv4jwAAAAAAAAABArkAgAAAAAAAAAAAaO9vOM0M1Ps7cbVoAwarn0H/USX8VUgN3hzKR27AH1wAAAAAAz5t7gKS/nQADGWcAAAABwAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuQB+AAAAAGQr+I8AAAAA",
                "hash": "f23e07e9b88ffdb04940fb8dfd625eb32dc19781896a101063f1a0975fc009f4",
                "id": "f23e07e9b88ffdb04940fb8dfd625eb32dc19781896a101063f1a0975fc009f4",
                "ledger": 45678720,
                "max_fee": "10000",
                "memo_type": "none",
                "operation_count": 1,
                "paging_token": "196188608523149312",
                "preconditions": {
                    "timebounds": {
                        "max_time": "1680603316",
                        "min_time": "0"
                    }
                },
                "result_meta_xdr": "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AAAAkvc7UYt//////////wAAAAEAAAABAAAALCs92rgAAAAvWHLrrwAAAAAAAAAAAAAAAwK5AH4AAAABAAAAAJCsmhShgYVbtY63wp2ri00EDG0TX4mik/kNZWFDADxlAAAAAUdCUFYAAAAAw+y5PPMHIkazPoP3+FxZAWpug05W+hSRi4g6//ynAQQAAACFxnU0Yn//////////AAAAAQAAAAEAAAAl6NtRowAAACSj+6KAAAAAAAAAAAAAAAABArkAgAAAAAEAAAAAkKyaFKGBhVu1jrfCnauLTQQMbRNfiaKT+Q1lYUMAPGUAAAABR0JQVgAAAADD7Lk88wciRrM+g/f4XFkBam6DTlb6FJGLiDr//KcBBAAAAIRxhO5if/////////8AAAABAAAAAQAAACXo21GjAAAAI08LXIAAAAAAAAAAAAAAAAMCuQB+AAAAAQAAAABo7284zQzU+ztxtWgDBqufQf9RJfxVSA3eHMpHbsAfXAAAAAFVU0RWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAAPfdNwM5//////////wAAAAEAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQK5AIAAAAABAAAAAGjvbzjNDNT7O3G1aAMGq59B/1El/FVIDd4cykduwB9cAAAAAVVTRFYAAAAAw+y5PPMHIkazPoP3+FxZAWpug05W+hSRi4g6//ynAQQAAAA8TP/rFn//////////AAAAAQAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADArkAfgAAAAEAAAAAaO9vOM0M1Ps7cbVoAwarn0H/USX8VUgN3hzKR27AH1wAAAABR0JQVgAAAADD7Lk88wciRrM+g/f4XFkBam6DTlb6FJGLiDr//KcBBAAAACa9sPxXf/////////8AAAABAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAECuQCAAAAAAQAAAABo7284zQzU+ztxtWgDBqufQf9RJfxVSA3eHMpHbsAfXAAAAAFHQlBWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAAKBKhQld//////////wAAAAEAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA==",
                "result_xdr": "AAAAAAAAJxAAAAAAAAAAAQAAAAAAAAAMAAAAAAAAAAIAAAABAAAAAJCsmhShgYVbtY63wp2ri00EDG0TX4mik/kNZWFDADxlAAAAAEleIfsAAAABR0JQVgAAAADD7Lk88wciRrM+g/f4XFkBam6DTlb6FJGLiDr//KcBBAAAAABPRjCAAAAAAVVTRFYAAAAAw+y5PPMHIkazPoP3+FxZAWpug05W+hSRi4g6//ynAQQAAAAAYxe8oAAAAAEAAAAAkKyaFKGBhVu1jrfCnauLTQQMbRNfiaKT+Q1lYUMAPGUAAAAASV4XRQAAAAFHQlBWAAAAAMPsuTzzByJGsz6D9/hcWQFqboNOVvoUkYuIOv/8pwEEAAAAAQWqFYAAAAABVVNEVgAAAADD7Lk88wciRrM+g/f4XFkBam6DTlb6FJGLiDr//KcBBAAAAAFHNhkYAAAAAgAAAAA=",
                "signatures": [
                    "AmwMLx7/HGzh95khPvaOr+sq9PuEyliGBi8ur7IKJ5QBjY3bImynfmh4nkqYaNcl9NmsbRYOkqISOlCbGJWYCA=="
                ],
                "source_account": "GBUO63ZYZUGNJ6Z3OG2WQAYGVOPUD72REX6FKSAN3YOMUR3OYAPVYOPU",
                "source_account_sequence": "185490308846085533",
                "successful": true,
                "valid_after": "1970-01-01T00:00:00Z",
                "valid_before": "2023-04-04T10:15:16Z"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/transactions?cursor=196188608523149312&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/transactions?cursor=196188608523145216&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/transactions?cursor=&limit=2&order=asc"
        }
    }
}
```

