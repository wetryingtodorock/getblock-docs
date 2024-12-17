---
title: zec:getblock \[POST\]
description: If verbosity is 0, returns a string that is serialized, hex-encoded datafor the block.If verbosity is 1, returns an Object with information about the block.If verbosity is 2, returns an Object with information about the blockand information about each transaction.
---

### Parameters


`hash|height` - string

The block hash or height. Height can be negative where -1 is the last
known valid block

`verbosity` - numeric

Optional, default is 1.

0 for hex encoded data, 1 for a json object, and 2 for json object with
transaction data.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblock",
"params": ["0000000000938f9fc631767d1302cd7a2cc29fce45f82724eb4d55d11658768f", 1],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "anchor": "318bcf0c2fad68a10606adba4704c457279ad68a6c82138721158a6ed73680a8",
        "bits": "1c028005",
        "chainhistoryroot": "a75b609ce1818c384cb651e0ecf733bc41fc9e731a788a9eacf5012bbc99d6c3",
        "chainwork": "00000000000000000000000000000000000000000000000006ca7f447fc62266",
        "confirmations": 236,
        "difficulty": 53685350.45312338,
        "finalsaplingroot": "5c14d2248db227e56eaa60f24aca1167bf6361aec8b998eb9beb10cfd7b47b69",
        "hash": "0000000000938f9fc631767d1302cd7a2cc29fce45f82724eb4d55d11658768f",
        "height": 1384123,
        "merkleroot": "e97acc0c3c6208a26e02b784ca6665d1944a9e7d159a714e894e97bb989414cb",
        "nextblockhash": "00000000010b5b439ac786033ce34541f460b6d4f98b36152031243938c7c20b",
        "nonce": "339102000000000000000000003d00000000000000000000000000005d555207",
        "previousblockhash": "000000000111846e3d6c31721cda040610437300dac7cdb856f719250571a37b",
        "size": 29544,
        "solution": "000642e5f02145f9517d20cacf903bf0360f3c237f272a69cb7b37c393f1bd27500d4daf6ad676b70c5007acbfd1c6cbd52b9bb071bfa8f304c180595173264411ad07592025bb3cb1b68470cb3473696d7ca69000602a1d4234297bbd53a8663ecd86b2429e9db25e1c9ed7f9bd8e84e28e3934ac5a4307c20989bcf6e10a0ae45dc6a55525f735ca3a50623b36aa801bb7f460e616f12d26065966e758b28d70de92af8c5feafd0056d8272dd99edfe0f5935f85ae240d494799705c07a7ed762f8bb03ac1fad10955c89260cefdff7186040e9b663b4bdb434edb79ad3563676f2376fd5c7d1a321dafb0d5acbdd02fb39bafb5f4adb6ba3e062c1a8a6d0a974f4642bbcaf5c2b4560b9b0b679cb895256389be95a63eef57e3e5992c3a2129d5eb964d133267a469b8114fd7031173d41944e3056f0fd1a29e35c7d36a119d82a7b5d477f152778d8672979d32e7007e24db81588452d7f0e15d4ec72b01fb1ef0e4cd77493f7c04ae2aa3f50998663fcbae86a3795c29a10404cc194d14e610bd7ab6a414e2971a169c540e8a0fa4d160ed8f88f1b8efc90fecfb35f3339d7b301c0680f7e0ee9121eb305ad216ba58e66b5cacbdda0355f8e5cea3d739892d9b75e1ddfbd206f3425f8da108a928aad29ba73b9d2e80b57bd24d8f3a14fea4e543d67488d29587f9b3e4157fa9ba79e2bf77d8606e01414030c742a17302b5882cc7cff132896b3732831084624a9f4c5d869b0f31c854cdac9551c7ee60f01e32a10474882254eb78a2a53b5c9f5bef5bffe2801e805d0c31ccb7edc4d8353b1ce555c192d517fdc602533613ab1a57f1c9efb2fe4ac8c0b205973271f5279503305125df03daa7b61d30bb8bd6ebd23ee8ca159419d48d1d1547777c24bf7747dc7af2611bd71a2fe35258645288d7808e9b7b2e5eb11b322bbbef3700f41ebc45dc000160fce95f396f06b69e685fe0d5301f53234e6a8a09bbe3966eb1d0923e509dff972d095aef216acaf15b76ef68941ed05c030269b8512c1b441767d5dcf329a356936ebefd60c1d8bc1af2b3086dd1f868ca394f3f7da10d3a580b4494c967b7c80a18d67fee8f25f1760ec768dbcfd22e6170bdf3330f54e439b8849a6bbb78416c26b9dda07b0496dd4135cbbcf3bf5c77e1dd4ec3a11124ff2d71e2b6411601ef9da433954a70cd76a482975a37961a2ab7898b06fcdc6892926e3d0355f08f265af2da20fcfe144614c4dfe2c8d47489708241bbbf8fa771d30ef806ff4737dda70499a64dfadbcad0385fa25f1e9a3c48df0286afec9ad3f032ded3065bd1f5585e13483669ff33163a7c2ad01564c9ba5347ca79fa4e91827a32f903766ddd2989068580f130b0ca20a1c076122e85e54b7b833176565217c2e5055a7841c0c6e917ba1c7d01d9758a0706e500755b55695bb4e8bf11d37dca082464fb7a7a673745a450a71112ec120e0150f465ca0404d5fe7850be3ddde7e2bda65c0b15c5628f6e761b0e58d994eba02168d618449deb750a6b0f973e9723b40dd93690cd96f54d0273415e794b2b43d97f997527177755b50453cc77fd9932f5222f98533dda9528806b4acb1a2f6d4f0614b01cb8412d52fb1cab8228bb6575f259b9490da03412337476a1bdfa535864079990fbf517f3718331c0ea52f1f8c90605f1ee60282e91c7f85dbff9fdc2043841ff356916f07737ff1a5d6ef97407ceddf9730cd694e7cdbb762a9f4acd35d31ebe9b1f6c71101258f4ebf62bd2718db48ab50839dde66e4347fc718a78d4b2fc49a78b059d99e01f31ddeff7123811ef0592199ba5a29a0673f05f0310211197cd2759cdde109bc3ed7f304f936dbfdaae2a0d6c5d659652f11ac814abb74680570f9259b175",
        "time": 1631173584,
        "tx": [
            "5db76e43724d980e01b5b98c9a83ba2d7fa565b3aa22bb3c5728ea56d0ed7cee",
            "62e278ff6a763a7adfbeb53689fab7bad235fa49eee746ddfbbc7453e8f6fc2e",
            "57682c60f21522665473f5c230636cf2fbe4c173a66e4216bb16e3753ba50711",
            "106f6b1e04785d2276bb5f90d4c3b841c2da401601ce595e330cfc58db689139",
            "0323496be043b41f8857dda04c423f6951927180bc756934c96c32a2c5e76254"
        ],
        "valuePools": [
            {
                "chainValue": 29342.43164115,
                "chainValueZat": 2934243164115,
                "id": "sprout",
                "monitored": true,
                "valueDelta": 0.0,
                "valueDeltaZat": 0
            },
            {
                "chainValue": 846950.61127337,
                "chainValueZat": 84695061127337,
                "id": "sapling",
                "monitored": true,
                "valueDelta": 8.00385238,
                "valueDeltaZat": 800385238
            }
        ],
        "version": 4
    }
}
```

