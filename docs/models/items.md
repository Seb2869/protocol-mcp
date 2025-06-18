# Items

## Example Usage

```typescript
import { Items } from "@rarible/protocol-mcp";

let value: Items = {
  items: [
    {
      id:
        "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
      blockchain: "ETHEREUM",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      tokenId: "123456",
      creators: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 663892,
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
      mintedAt: new Date("2025-12-13T16:57:11.570Z"),
      lastUpdatedAt: new Date("2025-03-25T00:05:48.099Z"),
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
            url: "https://unfortunate-tackle.biz/",
            representation: "ORIGINAL",
            mimeType: "image/png",
          },
        ],
        extraContent: [
          {
            url: "https://brown-makeover.com/",
            representation: "PREVIEW",
            mimeType: "image/png",
          },
        ],
      },
      deleted: false,
      bestSellOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "OBJKT",
        status: "INACTIVE",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2024-01-11T10:55:31.910Z"),
        lastUpdatedAt: new Date("2023-02-22T14:58:39.910Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "CRYPTO_PUNKS",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: 904519,
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "ETH",
            blockchain: "ETHEREUM",
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
      bestBidOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "CRYPTO_PUNKS",
        status: "CANCELLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2023-09-07T01:49:09.976Z"),
        lastUpdatedAt: new Date("2024-07-15T15:58:59.092Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "CURRENCY_TOKEN",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          },
          value: "123456.789",
        },
        take: {
          type: {
            blockchain: "ETHEREUM",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            atType: "CURRENCY_NATIVE",
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
      bestBidOrdersByCurrency: [
        {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "FXHASH",
          status: "FILLED",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2023-04-16T16:35:19.869Z"),
          lastUpdatedAt: new Date("2023-06-12T10:17:04.168Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              atType: "COLLECTION",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            },
            value: "123456.789",
          },
          take: {
            type: {
              atType: "ETH",
              blockchain: "ETHEREUM",
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
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 642434,
              },
            ],
            originFees: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 601874,
              },
            ],
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
            platform: "OPEN_SEA",
            status: "FILLED",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2024-08-19T12:05:12.090Z"),
            lastUpdatedAt: new Date("2023-05-31T10:07:56.733Z"),
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
                uri: "https://unrealistic-pressure.com/",
                creators: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 200313,
                  },
                ],
                royalties: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 437837,
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
                  value: 549541,
                },
              ],
              originFees: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 323075,
                },
              ],
            },
          },
          bestBidOrder: {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "FXHASH",
            status: "INACTIVE",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2024-11-02T15:39:47.415Z"),
            lastUpdatedAt: new Date("2023-08-21T10:25:10.554Z"),
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
                atType: "CURRENCY_TOKEN",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              },
              value: "123456.789",
            },
            salt: "<value>",
            feeTakers: [
              "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            ],
            data: {
              atType: "SOLANA_AUCTION_HOUSE_V1",
              auctionHouse:
                "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            },
          },
        },
      ],
      totalStock: "123456",
      sellers: 116860,
      lastSale: {
        date: new Date("2024-01-08T19:22:45.359Z"),
        seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: "123456.789",
        currency: {
          atType: "COLLECTION",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
          platform: "FXHASH",
          status: "ACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-08-10T12:28:19.855Z"),
          lastUpdatedAt: new Date("2024-06-04T03:38:04.541Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              atType: "ERC721",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
              tokenId: "123456",
            },
            value: "123456.789",
          },
          take: {
            type: {
              blockchain: "ETHEREUM",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              atType: "CURRENCY_NATIVE",
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
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 50156,
              },
            ],
            originFees: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 589555,
              },
            ],
          },
        },
        bestSellOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "IMMUTABLEX",
          status: "INACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-06-13T07:42:09.287Z"),
          lastUpdatedAt: new Date("2025-07-22T13:56:34.791Z"),
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
              atType: "ETH",
              blockchain: "ETHEREUM",
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
| `items`                                                                                                                                                        | [models.Item](../models/item.md)[]                                                                                                                             | :heavy_check_mark:                                                                                                                                             | List of found items                                                                                                                                            |