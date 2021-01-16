Specification for a [Graph project](https://thegraph.com/) subgraph which indexes [kiancoin](https://github.com/fafrd/kiancoin) transfers. Using this, I’m able to build the Top Holders list on [kiancoin.com](https://kiancoin.com).

Graph works off GraphQL queries. For example, given this query:

```graphql
{
    transfers {
        id
        from
        to
        value
    }
}
````

the graph node returns the following:
```json
{
  "data": {
    "transfers": [
      {
        "from": "0xbdb6eb461e9602ab64ca5e805a3906dbc1095250",
        "id": "0x0b758454a0a75256ef4e2a451aacfa7a38df5a6fb2ae6a0b74c6c1eb897ebc96-164",
        "to": "0x636483cb4e3e09e4a8e9d7f618a7f544579cc38c",
        "value": "28775800000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0x260bc9ab66cff1994904205278827af3a58546e965ab97c2901c9f2ad0404ab7-214",
        "to": "0x636483cb4e3e09e4a8e9d7f618a7f544579cc38c",
        "value": "2000000000000000"
      },
      {
        "from": "0x122fed718c784ad25e2a5ab351f034fc57512a48",
        "id": "0x33dfd0bea56ddb6a661a26a61adc42f7bcb381149cf3e869f0771fa8122ce289-98",
        "to": "0xbc31fda98ed7cf6daaf50327d922b78cbc486d23",
        "value": "32000000000000000"
      },
      {
        "from": "0x0000000000000000000000000000000000000000",
        "id": "0x4a17f2e9396052e5b1b3e1bbfaae1e57fc1ea84672032c3fbc97ee76448ad0db-31",
        "to": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "value": "1000000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0x6224252d651934c1108705d59bf3f7543f0dbc124fcaa42d19223ab57af9bffb-224",
        "to": "0x08b4249c79215fdd6a048af43e9ff86b9ee6be2e",
        "value": "50000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0x6575739bf8435df689fdc71428126ecb224e0912eb646772f423ccf98b970ec1-253",
        "to": "0x4c71526d3f7b112aaa4c0af173a6a47ab69d54cd",
        "value": "33000000000000000"
      },
      {
        "from": "0x122fed718c784ad25e2a5ab351f034fc57512a48",
        "id": "0x81f6b746f57256e8441a0930965b38f8ddfea939e5e02dad05141936e5b192ff-75",
        "to": "0x636483cb4e3e09e4a8e9d7f618a7f544579cc38c",
        "value": "80000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xcbf8c2cd79d7bee7616f30635822f28465a14a77ec5491ef4746cf0b44335401-209",
        "to": "0xe3a2b4da15130c7830862e945a2383f0a29b8bc8",
        "value": "110000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xcea89a5152601a0568add12aa6f3778ce70770b5f44cc06dddac0a31f8f81760-59",
        "to": "0x636483cb4e3e09e4a8e9d7f618a7f544579cc38c",
        "value": "80000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xdaa5920845ca7e5ca57fdb8e99c52960e0da22fae8eb2659e59ed1c484228076-245",
        "to": "0x969b81bba3a3eae0fccc78f8b64f012fd823a912",
        "value": "30000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xdf01312dbd6ea06129debf23262ab8235f82ed1092f8671dd18ff68143c2b7ae-145",
        "to": "0xbdb6eb461e9602ab64ca5e805a3906dbc1095250",
        "value": "100000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xe15366c481dbd0a5258c249deee618de3999922876a77d869e24f72fd10ca7d6-209",
        "to": "0xfc6f9a3c0fe29423ca6b974109817a323998f762",
        "value": "90000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xef08486909447597f108b3c4fdd3ade07f9fcfeb9e32d8eed0b136bae0764523-231",
        "to": "0x73bd1162e9da1b551d4601acf83158f3ac2247a9",
        "value": "100000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xf06e78c8fe7115541066b64cb2a123341483945fe21c60bd23d69fc6b04bfdc7-161",
        "to": "0xff82289231128fc6f185137f445d34e30d036c98",
        "value": "70000000000000000"
      },
      {
        "from": "0x5295b474f3a0bb39418456c96d6fcf13901a4aa1",
        "id": "0xf540d2db173bd1441a89e85fc308de220a7aa645d390798780c4f6f765382ae0-192",
        "to": "0x122fed718c784ad25e2a5ab351f034fc57512a48",
        "value": "333000000000000000"
      }
    ]
  }
}
```
