# Collection

## Example Usage

```typescript
import { Collection } from "@rarible/protocol-mcp";

let value: Collection = {
  id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  parent: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  blockchain: "ETHEREUM",
  type: "ERC721",
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
        url: "https://young-duffel.name",
        representation: "PREVIEW",
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
    createdAt: new Date("2023-02-23T06:42:10.391Z"),
    lastUpdatedAt: new Date("2025-10-08T00:35:18.391Z"),
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
        atType: "SOLANA_NFT",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
      atType: "ETH_RARIBLE_V1",
      fee: "123456",
    },
  },
  bestSellOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "VERSUM",
    status: "ACTIVE",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2024-07-12T01:14:58.792Z"),
    lastUpdatedAt: new Date("2025-05-31T20:02:23.819Z"),
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
      atType: "IMMUTABLEX_RARIBLE_V1",
      payouts: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 619875,
        },
      ],
      originFees: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 857724,
        },
      ],
    },
  },
  bestBidOrdersByCurrency: [
    {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "TEIA",
      status: "CANCELLED",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2023-10-04T14:50:09.018Z"),
      lastUpdatedAt: new Date("2023-12-18T00:05:55.713Z"),
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
        atType: "ETH_BASIC_SEAPORT_DATA_V1",
        protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        orderType: "FULL_RESTRICTED",
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
            itemType: "NATIVE",
            token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            identifierOrCriteria: "123456",
            startAmount: "123456",
            endAmount: "123456",
            recipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
        platform: "RARIBLE",
        status: "FILLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2025-06-21T16:48:18.921Z"),
        lastUpdatedAt: new Date("2025-05-27T22:54:21.916Z"),
        makePrice: "123456.789",
        takePrice: "123456.789",
        makePriceUsd: "123456.789",
        takePriceUsd: "123456.789",
        maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        make: {
          type: {
            atType: "NFT",
            collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            itemId:
              "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "ERC1155",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: "123456",
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
        platform: "RARIBLE",
        status: "CANCELLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2025-12-21T20:31:55.605Z"),
        lastUpdatedAt: new Date("2024-10-29T21:36:12.084Z"),
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
            atType: "SOLANA_SOL",
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
          feeMethod: "PROTOCOL_FEE",
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                                                                                                                                                                                        | Type                                                                                                                                                                                                                                                                                                                                                         | Required                                                                                                                                                                                                                                                                                                                                                     | Description                                                                                                                                                                                                                                                                                                                                                  | Example                                                                                                                                                                                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                                                                                                                                                                                         | *string*                                                                                                                                                                                                                                                                                                                                                     | :heavy_check_mark:                                                                                                                                                                                                                                                                                                                                           | Collection id                                                                                                                                                                                                                                                                                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                                                                                                                                                                                                                                                                                          |
| `parent`                                                                                                                                                                                                                                                                                                                                                     | *string*                                                                                                                                                                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | Collection id                                                                                                                                                                                                                                                                                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                                                                                                                                                                                                                                                                                          |
| `blockchain`                                                                                                                                                                                                                                                                                                                                                 | [models.Blockchain](../models/blockchain.md)                                                                                                                                                                                                                                                                                                                 | :heavy_check_mark:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          | ETHEREUM                                                                                                                                                                                                                                                                                                                                                     |
| `structure`                                                                                                                                                                                                                                                                                                                                                  | [models.Structure](../models/structure.md)                                                                                                                                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | Collection structure can be described as:<br/>- REGULAR: a standalone collection that has a corresponding contract address on the blockchain.<br/>- COMPOSITE: an artificial collection that is composed of one or more regular collections or items.<br/>- PART: an artificial collection that is a part of a larger regular collection, thus has a parent collection.<br/> |                                                                                                                                                                                                                                                                                                                                                              |
| `type`                                                                                                                                                                                                                                                                                                                                                       | [models.CollectionType](../models/collectiontype.md)                                                                                                                                                                                                                                                                                                         | :heavy_check_mark:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `status`                                                                                                                                                                                                                                                                                                                                                     | [models.Status](../models/status.md)                                                                                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `name`                                                                                                                                                                                                                                                                                                                                                       | *string*                                                                                                                                                                                                                                                                                                                                                     | :heavy_check_mark:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `symbol`                                                                                                                                                                                                                                                                                                                                                     | *string*                                                                                                                                                                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `owner`                                                                                                                                                                                                                                                                                                                                                      | *string*                                                                                                                                                                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | Blockchain address in Union format `${blockchainGroup}:${token}`                                                                                                                                                                                                                                                                                             | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                                                                                                                                                                                                                                                                                          |
| `features`                                                                                                                                                                                                                                                                                                                                                   | [models.CollectionFeature](../models/collectionfeature.md)[]                                                                                                                                                                                                                                                                                                 | :heavy_check_mark:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `minters`                                                                                                                                                                                                                                                                                                                                                    | *string*[]                                                                                                                                                                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | List of addresses that can mint items in this collection                                                                                                                                                                                                                                                                                                     |                                                                                                                                                                                                                                                                                                                                                              |
| `meta`                                                                                                                                                                                                                                                                                                                                                       | [models.CollectionMeta](../models/collectionmeta.md)                                                                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `bestBidOrder`                                                                                                                                                                                                                                                                                                                                               | [models.Order](../models/order.md)                                                                                                                                                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `bestSellOrder`                                                                                                                                                                                                                                                                                                                                              | [models.Order](../models/order.md)                                                                                                                                                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `bestBidOrdersByCurrency`                                                                                                                                                                                                                                                                                                                                    | [models.Order](../models/order.md)[]                                                                                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | Contains best bid order for each currency if exists                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `originOrders`                                                                                                                                                                                                                                                                                                                                               | [models.OriginOrders](../models/originorders.md)[]                                                                                                                                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `self`                                                                                                                                                                                                                                                                                                                                                       | *boolean*                                                                                                                                                                                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| ~~`scam`~~                                                                                                                                                                                                                                                                                                                                                   | *boolean*                                                                                                                                                                                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | : warning: ** DEPRECATED **: This will be removed in a future release, please migrate away from it as soon as possible.<br/><br/>Deprecated, use spamScore instead                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                              |
| `spamScore`                                                                                                                                                                                                                                                                                                                                                  | *number*                                                                                                                                                                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | Spam score of the collection, 0 - not spam, 100 - spam                                                                                                                                                                                                                                                                                                       |                                                                                                                                                                                                                                                                                                                                                              |
| `hasTraits`                                                                                                                                                                                                                                                                                                                                                  | *boolean*                                                                                                                                                                                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `shared`                                                                                                                                                                                                                                                                                                                                                     | *boolean*                                                                                                                                                                                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |
| `extra`                                                                                                                                                                                                                                                                                                                                                      | Record<string, *string*>                                                                                                                                                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | Blockchain-specific information about this NFT collection particular to that blockchain's data model                                                                                                                                                                                                                                                         |                                                                                                                                                                                                                                                                                                                                                              |
| `version`                                                                                                                                                                                                                                                                                                                                                    | *number*                                                                                                                                                                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                              |