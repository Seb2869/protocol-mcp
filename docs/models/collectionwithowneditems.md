# CollectionWithOwnedItems

## Example Usage

```typescript
import { CollectionWithOwnedItems } from "@rarible/protocol-mcp";

let value: CollectionWithOwnedItems = {
  collection: {
    id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    parent: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    blockchain: "ETHEREUM",
    type: "ERC1155",
    name: "<value>",
    owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    features: [
      "PAUSABLE",
    ],
    minters: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    meta: {
      name: "<value>",
      content: [
        {
          url: "https://radiant-quinoa.biz/",
          representation: "PORTRAIT",
          mimeType: "image/png",
        },
      ],
      feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    },
    bestBidOrder: {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "OTHER",
      status: "ACTIVE",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2025-05-10T21:00:40.208Z"),
      lastUpdatedAt: new Date("2023-02-07T07:22:29.103Z"),
      makePrice: "123456.789",
      takePrice: "123456.789",
      makePriceUsd: "123456.789",
      takePriceUsd: "123456.789",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        type: {
          blockchain: "ETHEREUM",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          atType: "CURRENCY_NATIVE",
        },
        value: "123456.789",
      },
      take: {
        type: {
          atType: "SOLANA_SOL",
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
    bestSellOrder: {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "CRYPTO_PUNKS",
      status: "ACTIVE",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2025-07-19T11:21:13.076Z"),
      lastUpdatedAt: new Date("2024-07-25T03:26:30.737Z"),
      makePrice: "123456.789",
      takePrice: "123456.789",
      makePriceUsd: "123456.789",
      takePriceUsd: "123456.789",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        type: {
          atType: "FLOW_FT",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        },
        value: "123456.789",
      },
      take: {
        type: {
          atType: "ERC20",
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
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 266467,
          },
        ],
        originFees: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 348928,
          },
        ],
      },
    },
    bestBidOrdersByCurrency: [
      {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "RARIBLE",
        status: "INACTIVE",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2023-05-23T20:40:43.276Z"),
        lastUpdatedAt: new Date("2023-10-11T13:48:43.829Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "FLOW_FT",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "NFT",
            collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 412365,
            },
          ],
          originFees: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 582143,
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
          platform: "OTHER",
          status: "CANCELLED",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2025-02-23T12:02:55.053Z"),
          lastUpdatedAt: new Date("2023-09-11T19:41:54.224Z"),
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
          platform: "OBJKT",
          status: "INACTIVE",
          makeStock: "123456.789",
          cancelled: false,
          createdAt: new Date("2024-01-10T09:12:19.774Z"),
          lastUpdatedAt: new Date("2023-06-10T04:49:48.280Z"),
          makePrice: "123456.789",
          takePrice: "123456.789",
          makePriceUsd: "123456.789",
          takePriceUsd: "123456.789",
          maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          make: {
            type: {
              blockchain: "ETHEREUM",
              contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
              atType: "CURRENCY_NATIVE",
            },
            value: "123456.789",
          },
          take: {
            type: {
              atType: "COLLECTION",
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
            atType: "FLOW_RARIBLE_V1",
            payouts: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 614536,
              },
            ],
            originFees: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 554283,
              },
            ],
          },
        },
      },
    ],
  },
  ownedItems: 405028,
};
```

## Fields

| Field                                        | Type                                         | Required                                     | Description                                  |
| -------------------------------------------- | -------------------------------------------- | -------------------------------------------- | -------------------------------------------- |
| `collection`                                 | [models.Collection](../models/collection.md) | :heavy_check_mark:                           | N/A                                          |
| `ownedItems`                                 | *number*                                     | :heavy_check_mark:                           | N/A                                          |