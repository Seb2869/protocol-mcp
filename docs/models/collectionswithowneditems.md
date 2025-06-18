# CollectionsWithOwnedItems

## Example Usage

```typescript
import { CollectionsWithOwnedItems } from "@rarible/protocol-mcp";

let value: CollectionsWithOwnedItems = {
  collections: [
    {
      collection: {
        id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        parent: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        blockchain: "ETHEREUM",
        type: "ERC1155",
        name: "<value>",
        owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        features: [
          "MINT_WITH_ADDRESS",
        ],
        minters: [
          "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        ],
        meta: {
          name: "<value>",
          content: [
            {
              url: "https://sophisticated-reward.com/",
              representation: "ORIGINAL",
              mimeType: "image/png",
            },
          ],
          feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        },
        bestBidOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "IMMUTABLEX",
          status: "CANCELLED",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2023-05-14T11:09:08.192Z"),
          lastUpdatedAt: new Date("2025-01-08T21:10:43.644Z"),
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
            atType: "ETH_RARIBLE_V1",
            fee: "123456",
          },
        },
        bestSellOrder: {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "HEN",
          status: "INACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-07-24T17:45:58.440Z"),
          lastUpdatedAt: new Date("2024-10-24T04:18:51.939Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              atType: "ERC1155_Lazy",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
              tokenId: "123456",
              uri: "https://faraway-pulse.com/",
              supply: "123456",
              creators: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 386340,
                },
              ],
              royalties: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 549993,
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
              atType: "NFT",
              collectionId:
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
            atType: "RAW",
          },
        },
        bestBidOrdersByCurrency: [
          {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "FXHASH",
            status: "INACTIVE",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2025-07-02T11:42:47.530Z"),
            lastUpdatedAt: new Date("2023-04-04T03:21:34.240Z"),
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
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
              platform: "OPEN_SEA",
              status: "FILLED",
              makeStock: "123456.789",
              cancelled: false,
              createdAt: new Date("2025-06-23T17:48:49.145Z"),
              lastUpdatedAt: new Date("2023-11-22T21:09:24.450Z"),
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
                  uri: "https://ironclad-baseboard.net",
                  supply: "123456",
                  creators: [
                    {
                      account:
                        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                      value: 993363,
                    },
                  ],
                  royalties: [
                    {
                      account:
                        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                      value: 341518,
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
                atType: "IMMUTABLEX_RARIBLE_V1",
                payouts: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 188983,
                  },
                ],
                originFees: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 233662,
                  },
                ],
              },
            },
            bestBidOrder: {
              id:
                "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
              fill: "123456.789",
              platform: "CRYPTO_PUNKS",
              status: "ACTIVE",
              makeStock: "123456.789",
              cancelled: false,
              createdAt: new Date("2025-10-09T17:46:39.764Z"),
              lastUpdatedAt: new Date("2024-10-30T13:28:38.037Z"),
              makePrice: "123456.789",
              takePrice: "123456.789",
              makePriceUsd: "123456.789",
              takePriceUsd: "123456.789",
              maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              make: {
                type: {
                  atType: "COLLECTION",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                  collection:
                    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                },
                value: "123456.789",
              },
              take: {
                type: {
                  atType: "ERC1155",
                  contract:
                    "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
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
                atType: "ETH_BASIC_SEAPORT_DATA_V1",
                protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                orderType: "FULL_RESTRICTED",
                offer: [
                  {
                    itemType: "NATIVE",
                    token:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    identifierOrCriteria: "123456",
                    startAmount: "123456",
                    endAmount: "123456",
                  },
                ],
                consideration: [
                  {
                    itemType: "ERC721_WITH_CRITERIA",
                    token:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    identifierOrCriteria: "123456",
                    startAmount: "123456",
                    endAmount: "123456",
                    recipient:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  },
                ],
                zone: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                zoneHash: "<value>",
                conduitKey: "<value>",
                nonce: "123456",
              },
            },
          },
        ],
      },
      ownedItems: 319337,
    },
  ],
};
```

## Fields

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `collections`                                                              | [models.CollectionWithOwnedItems](../models/collectionwithowneditems.md)[] | :heavy_check_mark:                                                         | N/A                                                                        |
| `continuation`                                                             | *string*                                                                   | :heavy_minus_sign:                                                         | Continuation token to paginate result                                      |