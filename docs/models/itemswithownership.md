# ItemsWithOwnership

## Example Usage

```typescript
import { ItemsWithOwnership } from "@rarible/protocol-mcp";

let value: ItemsWithOwnership = {
  items: [
    {
      item: {
        id:
          "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
        blockchain: "ETHEREUM",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        tokenId: "123456",
        creators: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 379157,
          },
        ],
        ownerIfSingle: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        lazySupply: "123456",
        pending: [
          {
            atType: "TRANSFER",
            from: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          },
        ],
        mintedAt: new Date("2025-04-19T01:41:10.886Z"),
        lastUpdatedAt: new Date("2025-07-25T02:31:20.112Z"),
        supply: "123456",
        meta: {
          name: "<value>",
          attributes: [
            {
              key: "<key>",
            },
          ],
          content: [
            {
              url: "https://worthless-descendant.com/",
              representation: "INITIAL",
              mimeType: "image/png",
            },
          ],
          extraContent: [
            {
              url: "https://shimmering-going.com/",
              representation: "INITIAL",
              mimeType: "image/png",
            },
          ],
        },
        deleted: false,
        bestSellOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "HEN",
          status: "INACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-09-23T02:05:58.443Z"),
          lastUpdatedAt: new Date("2023-04-27T09:30:02.371Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              atType: "ERC20",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            },
            value: "123456.789",
          },
          take: {
            type: {
              atType: "NFT_OF_COLLECTION",
              collectionId:
                "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            },
            value: "123456.789",
          },
          salt: "<value>",
          feeTakers: [
            "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          ],
          data: {
            atType: "ETH_CRYPTO_PUNKS",
            stub: "STUB",
          },
        },
        bestBidOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "OTHER",
          status: "ACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2024-08-06T21:25:35.008Z"),
          lastUpdatedAt: new Date("2024-04-18T23:47:21.436Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              atType: "SOLANA_NFT",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
              itemId:
                "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
            },
            value: "123456.789",
          },
          take: {
            type: {
              atType: "SOLANA_FT",
              address: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            },
            value: "123456.789",
          },
          salt: "<value>",
          feeTakers: [
            "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          ],
          data: {
            atType: "SOLANA_AUCTION_HOUSE_V1",
            auctionHouse: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          },
        },
        bestBidOrdersByCurrency: [
          {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "VERSUM",
            status: "FILLED",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2025-12-01T09:59:56.687Z"),
            lastUpdatedAt: new Date("2024-01-23T10:13:19.163Z"),
            makePrice: "123456.789",
            takePrice: "123456.789",
            makePriceUsd: "123456.789",
            takePriceUsd: "123456.789",
            maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            make: {
              type: {
                atType: "SOLANA_NFT",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                itemId:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
              },
              value: "123456.789",
            },
            take: {
              type: {
                atType: "GEN_ART",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
              },
              value: "123456.789",
            },
            salt: "<value>",
            feeTakers: [
              "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            ],
            data: {
              atType: "ETH_CRYPTO_PUNKS",
              stub: "STUB",
            },
          },
        ],
        originOrders: [
          {
            origin: "<value>",
            bestSellOrder: {
              id:
                "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
              fill: "123456.789",
              platform: "FXHASH",
              status: "FILLED",
              makeStock: "123456.789",
              cancelled: false,
              createdAt: new Date("2023-07-10T08:44:27.903Z"),
              lastUpdatedAt: new Date("2024-02-01T00:42:32.096Z"),
              makePrice: "123456.789",
              takePrice: "123456.789",
              makePriceUsd: "123456.789",
              takePriceUsd: "123456.789",
              maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              make: {
                type: {
                  atType: "ERC20",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                },
                value: "123456.789",
              },
              take: {
                type: {
                  atType: "SOLANA_FT",
                  address:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                },
                value: "123456.789",
              },
              salt: "<value>",
              feeTakers: [
                "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              ],
              data: {
                atType: "FLOW_RARIBLE_V1",
                payouts: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 868534,
                  },
                ],
                originFees: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 518848,
                  },
                ],
              },
            },
            bestBidOrder: {
              id:
                "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
              fill: "123456.789",
              platform: "RARIBLE",
              status: "FILLED",
              makeStock: "123456.789",
              cancelled: false,
              createdAt: new Date("2024-07-04T17:00:47.946Z"),
              lastUpdatedAt: new Date("2025-09-19T05:40:47.714Z"),
              makePrice: "123456.789",
              takePrice: "123456.789",
              makePriceUsd: "123456.789",
              takePriceUsd: "123456.789",
              maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              make: {
                type: {
                  atType: "ERC1155_Lazy",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                  collection:
                    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                  tokenId: "123456",
                  uri: "https://broken-hovercraft.name",
                  supply: "123456",
                  creators: [
                    {
                      account:
                        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                      value: 955697,
                    },
                  ],
                  royalties: [
                    {
                      account:
                        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                      value: 932761,
                    },
                  ],
                  signatures: [
                    "<value>",
                  ],
                },
                value: "123456.789",
              },
              take: {
                type: {
                  atType: "ERC1155_Lazy",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                  collection:
                    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                  tokenId: "123456",
                  uri: "https://honored-bench.biz/",
                  supply: "123456",
                  creators: [
                    {
                      account:
                        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                      value: 264067,
                    },
                  ],
                  royalties: [
                    {
                      account:
                        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                      value: 600761,
                    },
                  ],
                  signatures: [
                    "<value>",
                  ],
                },
                value: "123456.789",
              },
              salt: "<value>",
              feeTakers: [
                "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              ],
              data: {
                atType: "FLOW_RARIBLE_V1",
                payouts: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 279325,
                  },
                ],
                originFees: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 944607,
                  },
                ],
              },
            },
          },
        ],
        totalStock: "123456",
        sellers: 225650,
        lastSale: {
          date: new Date("2025-06-13T07:01:47.948Z"),
          seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: "123456.789",
          currency: {
            atType: "SOLANA_NFT",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            itemId:
              "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
          },
          price: "123456.789",
        },
        itemCollection: {
          id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          name: "<value>",
          bestBidOrder: {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "OTHER",
            status: "FILLED",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2025-10-02T15:45:13.574Z"),
            lastUpdatedAt: new Date("2023-06-27T23:08:38.891Z"),
            makePrice: "123456.789",
            takePrice: "123456.789",
            makePriceUsd: "123456.789",
            takePriceUsd: "123456.789",
            maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            make: {
              type: {
                atType: "ERC721_Lazy",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                tokenId: "123456",
                uri: "https://superior-issue.net",
                creators: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 773886,
                  },
                ],
                royalties: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 760731,
                  },
                ],
                signatures: [
                  "<value>",
                ],
              },
              value: "123456.789",
            },
            take: {
              type: {
                atType: "FLOW_FT",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              },
              value: "123456.789",
            },
            salt: "<value>",
            feeTakers: [
              "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            ],
            data: {
              atType: "IMMUTABLEX_RARIBLE_V1",
              payouts: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 959244,
                },
              ],
              originFees: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 232891,
                },
              ],
            },
          },
          bestSellOrder: {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "OBJKT",
            status: "ACTIVE",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2024-03-04T21:39:06.212Z"),
            lastUpdatedAt: new Date("2023-07-28T01:53:57.589Z"),
            makePrice: "123456.789",
            takePrice: "123456.789",
            makePriceUsd: "123456.789",
            takePriceUsd: "123456.789",
            maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            make: {
              type: {
                atType: "SOLANA_FT",
                address: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              },
              value: "123456.789",
            },
            take: {
              type: {
                atType: "ERC721_Lazy",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                tokenId: "123456",
                uri: "https://unlucky-swine.org",
                creators: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 565227,
                  },
                ],
                royalties: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 265394,
                  },
                ],
                signatures: [
                  "<value>",
                ],
              },
              value: "123456.789",
            },
            salt: "<value>",
            feeTakers: [
              "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            ],
            data: {
              atType: "IMMUTABLEX_RARIBLE_V1",
              payouts: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 846654,
                },
              ],
              originFees: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 503575,
                },
              ],
            },
          },
        },
      },
      ownership: {
        id:
          "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410:0x4765273c477c2dc484da4f1984639e943adccfeb",
        blockchain: "ETHEREUM",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: "123456",
        createdAt: new Date("2025-06-07T23:06:42.665Z"),
        creators: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 867852,
          },
        ],
        lazyValue: "123456",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ~~`total`~~                                                                                                                                                    | *number*                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                             | : warning: ** DEPRECATED **: This will be removed in a future release, please migrate away from it as soon as possible.<br/><br/>Number of items were found by request |
| `continuation`                                                                                                                                                 | *string*                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                             | Continuation token to paginate items search result                                                                                                             |
| `items`                                                                                                                                                        | [models.ItemWithOwnership](../models/itemwithownership.md)[]                                                                                                   | :heavy_check_mark:                                                                                                                                             | List of found items                                                                                                                                            |