# Collections

## Example Usage

```typescript
import { Collections } from "@rarible/protocol-mcp";

let value: Collections = {
  collections: [
    {
      id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      parent: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      blockchain: "ETHEREUM",
      type: "TOKEN_GROUP_2022",
      name: "<value>",
      owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      features: [
        "BURN",
      ],
      minters: [
        "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      ],
      meta: {
        name: "<value>",
        content: [
          {
            url: "https://muffled-backburn.name",
            representation: "INITIAL",
            mimeType: "image/png",
          },
        ],
        feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      },
      bestBidOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "HEN",
        status: "INACTIVE",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2024-10-26T10:35:51.417Z"),
        lastUpdatedAt: new Date("2025-02-02T20:36:30.567Z"),
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
            atType: "NFT_OF_COLLECTION",
            collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
          side: "BUY",
          saleKind: "DUTCH_AUCTION",
          howToCall: "CALL",
          callData: "<value>",
          replacementPattern: "<value>",
          staticTarget: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          staticExtraData: "<value>",
          extra: "123456",
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
        createdAt: new Date("2024-11-28T19:58:13.274Z"),
        lastUpdatedAt: new Date("2025-01-30T21:29:11.474Z"),
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
            collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 650242,
            },
          ],
          originFees: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 787867,
            },
          ],
        },
      },
      bestBidOrdersByCurrency: [
        {
          id:
            "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
          fill: "123456.789",
          platform: "FXHASH",
          status: "ACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2024-03-06T10:45:39.462Z"),
          lastUpdatedAt: new Date("2025-09-15T21:32:45.871Z"),
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
            atType: "ETH_BASIC_SEAPORT_DATA_V1",
            protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            orderType: "CONTRACT",
            offer: [
              {
                itemType: "ERC20",
                token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                identifierOrCriteria: "123456",
                startAmount: "123456",
                endAmount: "123456",
              },
            ],
            consideration: [
              {
                itemType: "ERC721_WITH_CRITERIA",
                token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
      ],
      originOrders: [
        {
          origin: "<value>",
          bestSellOrder: {
            id:
              "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
            fill: "123456.789",
            platform: "OPEN_SEA",
            status: "CANCELLED",
            makeStock: "123456.789",
            cancelled: false,
            createdAt: new Date("2025-12-01T07:21:24.751Z"),
            lastUpdatedAt: new Date("2024-12-01T08:52:12.423Z"),
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
                atType: "ERC721_Lazy",
                contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
                collection:
                  "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
                tokenId: "123456",
                uri: "https://stable-fort.org/",
                creators: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 16323,
                  },
                ],
                royalties: [
                  {
                    account:
                      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                    value: 30081,
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
              atType: "SOLANA_AUCTION_HOUSE_V1",
              auctionHouse:
                "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
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
            createdAt: new Date("2023-08-13T22:11:17.098Z"),
            lastUpdatedAt: new Date("2024-04-09T22:31:02.902Z"),
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
                  value: 451585,
                },
              ],
              originFees: [
                {
                  account:
                    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                  value: 182872,
                },
              ],
            },
          },
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                               | Type                                                                                                                                                                | Required                                                                                                                                                            | Description                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ~~`total`~~                                                                                                                                                         | *number*                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                  | : warning: ** DEPRECATED **: This will be removed in a future release, please migrate away from it as soon as possible.<br/><br/>Number of ownerships were found by request |
| `continuation`                                                                                                                                                      | *string*                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                  | Continuation token to paginate collections search result                                                                                                            |
| `collections`                                                                                                                                                       | [models.Collection](../models/collection.md)[]                                                                                                                      | :heavy_check_mark:                                                                                                                                                  | N/A                                                                                                                                                                 |