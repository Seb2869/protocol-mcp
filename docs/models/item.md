# Item

## Example Usage

```typescript
import { Item } from "@rarible/protocol-mcp";

let value: Item = {
  id:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  blockchain: "ETHEREUM",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  tokenId: "123456",
  creators: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 424912,
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
  mintedAt: new Date("2024-09-18T18:35:17.981Z"),
  lastUpdatedAt: new Date("2025-03-05T12:53:50.183Z"),
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
        url: "https://cautious-lift.net/",
        representation: "PREVIEW",
        mimeType: "image/png",
      },
    ],
    extraContent: [
      {
        url: "https://evil-packaging.net/",
        representation: "BIG",
        mimeType: "image/png",
      },
    ],
  },
  deleted: false,
  bestSellOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "VERSUM",
    status: "ACTIVE",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2025-03-14T16:07:24.463Z"),
    lastUpdatedAt: new Date("2023-02-14T23:23:26.093Z"),
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
          itemType: "ERC20",
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
  bestBidOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "OBJKT",
    status: "INACTIVE",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2024-12-30T10:23:56.324Z"),
    lastUpdatedAt: new Date("2025-01-11T17:34:04.239Z"),
    makePrice: "123456.789",
    takePrice: "123456.789",
    makePriceUsd: "123456.789",
    takePriceUsd: "123456.789",
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    make: {
      type: {
        atType: "FLOW_NFT",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        tokenId: "123456",
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
      howToCall: "DELEGATE_CALL",
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
      platform: "VERSUM",
      status: "CANCELLED",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2025-01-13T12:00:23.863Z"),
      lastUpdatedAt: new Date("2024-12-11T16:43:26.523Z"),
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
        atType: "ETH_BASIC_SEAPORT_DATA_V1",
        protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        orderType: "FULL_RESTRICTED",
        offer: [
          {
            itemType: "ERC721",
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
        status: "ACTIVE",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2024-04-18T17:59:33.943Z"),
        lastUpdatedAt: new Date("2024-10-24T16:10:31.900Z"),
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
            tokenId: 61388,
          },
          value: "123456.789",
        },
        take: {
          type: {
            atType: "ERC721",
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
          atType: "ETH_CRYPTO_PUNKS",
          stub: "STUB",
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
        createdAt: new Date("2024-07-22T07:07:22.880Z"),
        lastUpdatedAt: new Date("2024-10-16T00:19:25.551Z"),
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
            atType: "ERC1155_Lazy",
            contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
            collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
            tokenId: "123456",
            uri: "https://rectangular-heartache.biz",
            supply: "123456",
            creators: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 210384,
              },
            ],
            royalties: [
              {
                account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
                value: 868872,
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
          atType: "ETH_CRYPTO_PUNKS",
          stub: "STUB",
        },
      },
    },
  ],
  totalStock: "123456",
  sellers: 59991,
  lastSale: {
    date: new Date("2023-02-17T04:51:43.976Z"),
    seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: "123456.789",
    currency: {
      atType: "CURRENCY_TOKEN",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
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
      platform: "OBJKT",
      status: "ACTIVE",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2025-04-24T02:04:13.676Z"),
      lastUpdatedAt: new Date("2023-03-26T01:54:46.970Z"),
      makePrice: "123456.789",
      takePrice: "123456.789",
      makePriceUsd: "123456.789",
      takePriceUsd: "123456.789",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        type: {
          atType: "FLOW_NFT",
          contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
          collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          tokenId: "123456",
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
        atType: "ETH_BASIC_SEAPORT_DATA_V1",
        protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        orderType: "CONTRACT",
        offer: [
          {
            itemType: "ERC721_WITH_CRITERIA",
            token: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            identifierOrCriteria: "123456",
            startAmount: "123456",
            endAmount: "123456",
          },
        ],
        consideration: [
          {
            itemType: "ERC1155",
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
    bestSellOrder: {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "TEIA",
      status: "INACTIVE",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2024-05-17T08:46:45.696Z"),
      lastUpdatedAt: new Date("2023-06-04T05:12:53.703Z"),
      makePrice: "123456.789",
      takePrice: "123456.789",
      makePriceUsd: "123456.789",
      takePriceUsd: "123456.789",
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      make: {
        type: {
          atType: "NFT_OF_COLLECTION",
          collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        },
        value: "123456.789",
      },
      take: {
        type: {
          atType: "FLOW_NFT",
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
        atType: "ETH_CRYPTO_PUNKS",
        stub: "STUB",
      },
    },
  },
};
```

## Fields

| Field                                                                                                                             | Type                                                                                                                              | Required                                                                                                                          | Description                                                                                                                       | Example                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                              | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | Item Id, has format `ETHEREUM:${token}:${tokenId}`                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410 |
| `blockchain`                                                                                                                      | [models.Blockchain](../models/blockchain.md)                                                                                      | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               | ETHEREUM                                                                                                                          |
| `collection`                                                                                                                      | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | Collection id                                                                                                                     | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                                                               |
| `contract`                                                                                                                        | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | Blockchain contract address in Union format `ETHEREUM:${token}`                                                                   | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                                                               |
| `tokenId`                                                                                                                         | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               | 123456                                                                                                                            |
| `creators`                                                                                                                        | [models.Creator](../models/creator.md)[]                                                                                          | :heavy_check_mark:                                                                                                                | Creators of the target item                                                                                                       |                                                                                                                                   |
| `ownerIfSingle`                                                                                                                   | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | Blockchain address in Union format `${blockchainGroup}:${token}`                                                                  | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                                                               |
| `ownerChangeDate`                                                                                                                 | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)                                     | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `lazySupply`                                                                                                                      | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               | 123456                                                                                                                            |
| `pending`                                                                                                                         | [models.ItemTransfer](../models/itemtransfer.md)[]                                                                                | :heavy_check_mark:                                                                                                                | Pending information about the item                                                                                                |                                                                                                                                   |
| `mintedAt`                                                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)                                     | :heavy_check_mark:                                                                                                                | Date and time of the item minting                                                                                                 |                                                                                                                                   |
| `lastUpdatedAt`                                                                                                                   | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)                                     | :heavy_check_mark:                                                                                                                | Filter condition to return only items that have been updated at this date                                                         |                                                                                                                                   |
| `supply`                                                                                                                          | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               | 123456                                                                                                                            |
| `meta`                                                                                                                            | [models.Meta](../models/meta.md)                                                                                                  | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `deleted`                                                                                                                         | *boolean*                                                                                                                         | :heavy_check_mark:                                                                                                                | Item was deleted or not                                                                                                           |                                                                                                                                   |
| `bestSellOrder`                                                                                                                   | [models.Order](../models/order.md)                                                                                                | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `bestBidOrder`                                                                                                                    | [models.Order](../models/order.md)                                                                                                | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `bestBidOrdersByCurrency`                                                                                                         | [models.Order](../models/order.md)[]                                                                                              | :heavy_minus_sign:                                                                                                                | Contains best bid order for each currency if exists                                                                               |                                                                                                                                   |
| `originOrders`                                                                                                                    | [models.OriginOrders](../models/originorders.md)[]                                                                                | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `totalStock`                                                                                                                      | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               | 123456                                                                                                                            |
| `sellers`                                                                                                                         | *number*                                                                                                                          | :heavy_check_mark:                                                                                                                | Total count of users selling this item ATM                                                                                        |                                                                                                                                   |
| `lastSale`                                                                                                                        | [models.ItemLastSale](../models/itemlastsale.md)                                                                                  | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `self`                                                                                                                            | *boolean*                                                                                                                         | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `suspicious`                                                                                                                      | *boolean*                                                                                                                         | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `itemCollection`                                                                                                                  | [models.ItemCollection](../models/itemcollection.md)                                                                              | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `features`                                                                                                                        | [models.ItemFeature](../models/itemfeature.md)[]                                                                                  | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `extra`                                                                                                                           | Record<string, *string*>                                                                                                          | :heavy_minus_sign:                                                                                                                | Blockchain-specific information about this NFT item particular to that blockchain's data model                                    |                                                                                                                                   |
| `version`                                                                                                                         | *number*                                                                                                                          | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |