# DuplicatedItemGroups

## Example Usage

```typescript
import { DuplicatedItemGroups } from "@rarible/protocol-mcp";

let value: DuplicatedItemGroups = {
  groups: [
    {
      traitGroups: [
        {
          key: "Hat",
          value: "Halo",
        },
      ],
      count: 996022,
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
            value: 99456,
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
        mintedAt: new Date("2025-09-13T10:53:03.615Z"),
        lastUpdatedAt: new Date("2025-11-22T02:36:13.211Z"),
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
              url: "https://cute-fen.org/",
              representation: "INITIAL",
              mimeType: "image/png",
            },
          ],
          extraContent: [
            {
              url: "https://lean-spirit.biz",
              representation: "PORTRAIT",
              mimeType: "image/png",
            },
          ],
        },
        deleted: false,
        bestSellOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "IMMUTABLEX",
          status: "CANCELLED",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2023-02-23T21:27:05.532Z"),
          lastUpdatedAt: new Date("2025-09-24T22:22:02.969Z"),
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
              atType: "GEN_ART",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
          platform: "VERSUM",
          status: "ACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-04-03T16:17:07.916Z"),
          lastUpdatedAt: new Date("2023-06-24T23:33:34.224Z"),
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
            atType: "ETH_OPEN_SEA_V1",
            exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            makerRelayerFee: "123456",
            takerRelayerFee: "123456",
            makerProtocolFee: "123456",
            takerProtocolFee: "123456",
            feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            feeMethod: "SPLIT_FEE",
            side: "SELL",
            saleKind: "FIXED_PRICE",
            howToCall: "CALL",
            callData: "<value>",
            replacementPattern: "<value>",
            staticTarget: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            staticExtraData: "<value>",
            extra: "123456",
          },
        },
        bestBidOrdersByCurrency: [
          {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "OBJKT",
            status: "FILLED",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2025-06-13T09:43:13.235Z"),
            lastUpdatedAt: new Date("2024-01-18T02:04:56.707Z"),
            makePrice: "123456.789",
            takePrice: "123456.789",
            makePriceUsd: "123456.789",
            takePriceUsd: "123456.789",
            maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            make: {
              type: {
                atType: "ETH",
                blockchain: "ETHEREUM",
              },
              value: "123456.789",
            },
            take: {
              type: {
                atType: "FLOW_NFT",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                tokenId: "123456",
              },
              value: "123456.789",
            },
            salt: "<value>",
            feeTakers: [
              "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            ],
            data: {
              atType: "ETH_RARIBLE_V2",
              payouts: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 670063,
                },
              ],
              originFees: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 582542,
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
              platform: "CRYPTO_PUNKS",
              status: "INACTIVE",
              makeStock: "123456.789",
              cancelled: false,
              createdAt: new Date("2024-12-13T11:19:27.230Z"),
              lastUpdatedAt: new Date("2023-03-24T01:46:29.679Z"),
              makePrice: "123456.789",
              takePrice: "123456.789",
              makePriceUsd: "123456.789",
              takePriceUsd: "123456.789",
              maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              make: {
                type: {
                  atType: "FLOW_FT",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                },
                value: "123456.789",
              },
              take: {
                type: {
                  atType: "SOLANA_NFT",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                  collection:
                    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                  itemId:
                    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
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
                    value: 997145,
                  },
                ],
                originFees: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 810344,
                  },
                ],
              },
            },
            bestBidOrder: {
              id:
                "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
              fill: "123456.789",
              platform: "TEIA",
              status: "ACTIVE",
              makeStock: "123456.789",
              cancelled: false,
              createdAt: new Date("2025-01-14T07:28:23.170Z"),
              lastUpdatedAt: new Date("2023-01-10T19:55:33.771Z"),
              makePrice: "123456.789",
              takePrice: "123456.789",
              makePriceUsd: "123456.789",
              takePriceUsd: "123456.789",
              maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              make: {
                type: {
                  atType: "NFT_OF_COLLECTION",
                  collectionId:
                    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                },
                value: "123456.789",
              },
              take: {
                type: {
                  atType: "COLLECTION",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
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
                atType: "FLOW_RARIBLE_V1",
                payouts: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 620392,
                  },
                ],
                originFees: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 54001,
                  },
                ],
              },
            },
          },
        ],
        totalStock: "123456",
        sellers: 549960,
        lastSale: {
          date: new Date("2024-07-09T16:00:27.943Z"),
          seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: "123456.789",
          currency: {
            atType: "CRYPTO_PUNKS",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: 448377,
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
            platform: "HEN",
            status: "CANCELLED",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2024-12-28T01:46:16.091Z"),
            lastUpdatedAt: new Date("2025-08-28T17:48:52.231Z"),
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
              atType: "ETH_OPEN_SEA_V1",
              exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              makerRelayerFee: "123456",
              takerRelayerFee: "123456",
              makerProtocolFee: "123456",
              takerProtocolFee: "123456",
              feeRecipient:
                "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              feeMethod: "SPLIT_FEE",
              side: "BUY",
              saleKind: "FIXED_PRICE",
              howToCall: "CALL",
              callData: "<value>",
              replacementPattern: "<value>",
              staticTarget:
                "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              staticExtraData: "<value>",
              extra: "123456",
            },
          },
          bestSellOrder: {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "HEN",
            status: "ACTIVE",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2023-12-22T09:40:02.591Z"),
            lastUpdatedAt: new Date("2024-08-06T17:13:13.196Z"),
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
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                tokenId: 497032,
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
                  value: 991075,
                },
              ],
              originFees: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 564858,
                },
              ],
            },
          },
        },
      },
    },
  ],
};
```

## Fields

| Field                                                  | Type                                                   | Required                                               | Description                                            |
| ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ |
| `continuation`                                         | *string*                                               | :heavy_minus_sign:                                     | Continuation token to paginate duplicates              |
| `groups`                                               | [models.DuplicatedItem](../models/duplicateditem.md)[] | :heavy_check_mark:                                     | List of duplicated item groups                         |