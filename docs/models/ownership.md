# Ownership

## Example Usage

```typescript
import { Ownership } from "@rarible/protocol-mcp";

let value: Ownership = {
  id:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410:0x4765273c477c2dc484da4f1984639e943adccfeb",
  blockchain: "ETHEREUM",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  value: "123456",
  createdAt: new Date("2023-03-09T21:59:57.541Z"),
  lazyValue: "123456",
  pending: [
    {
      atType: "ROYALTY",
      royalties: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 230446,
        },
      ],
      owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      tokenId: "123456",
      value: "123456",
      date: new Date("2024-09-11T23:22:54.567Z"),
    },
  ],
  bestSellOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "HEN",
    status: "INACTIVE",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2025-11-03T07:00:15.938Z"),
    lastUpdatedAt: new Date("2023-08-01T23:43:13.775Z"),
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
        atType: "ERC1155_Lazy",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        tokenId: "123456",
        uri: "https://puny-maestro.info/",
        supply: "123456",
        creators: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 172177,
          },
        ],
        royalties: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 631066,
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
      atType: "RAW",
    },
  },
  originOrders: [
    {
      origin: "<value>",
      bestSellOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "TEIA",
        status: "FILLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2025-09-29T21:18:39.991Z"),
        lastUpdatedAt: new Date("2024-07-26T03:51:31.799Z"),
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
          atType: "ETH_BASIC_SEAPORT_DATA_V1",
          protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          orderType: "FULL_RESTRICTED",
          offer: [
            {
              itemType: "ERC1155_WITH_CRITERIA",
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
      bestBidOrder: {
        id:
          "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
        fill: "123456.789",
        platform: "OPEN_SEA",
        status: "CANCELLED",
        makeStock: "123456.789",
        cancelled: false,
        createdAt: new Date("2025-04-11T18:30:02.719Z"),
        lastUpdatedAt: new Date("2023-06-06T12:47:42.066Z"),
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
            atType: "SOLANA_SOL",
          },
          value: "123456.789",
        },
        salt: "<value>",
        feeTakers: [
          "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        ],
        data: {
          atType: "ETH_RARIBLE_V2_DATA_V3_BUY",
          payout: {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 378926,
          },
          originFeeFirst: {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 264507,
          },
          originFeeSecond: {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 900519,
          },
        },
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                        | Type                                                                                                                                                                         | Required                                                                                                                                                                     | Description                                                                                                                                                                  | Example                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                         | *string*                                                                                                                                                                     | :heavy_check_mark:                                                                                                                                                           | N/A                                                                                                                                                                          | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410:0x4765273c477c2dc484da4f1984639e943adccfeb |
| `blockchain`                                                                                                                                                                 | [models.Blockchain](../models/blockchain.md)                                                                                                                                 | :heavy_check_mark:                                                                                                                                                           | N/A                                                                                                                                                                          | ETHEREUM                                                                                                                                                                     |
| `itemId`                                                                                                                                                                     | *string*                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                           | Item Id, has format `ETHEREUM:${token}:${tokenId}`                                                                                                                           | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410                                            |
| `contract`                                                                                                                                                                   | *string*                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                           | Blockchain contract address in Union format `ETHEREUM:${token}`                                                                                                              | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                                                                                                          |
| `collection`                                                                                                                                                                 | *string*                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                           | Collection id                                                                                                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                                                                                                          |
| `tokenId`                                                                                                                                                                    | *string*                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          | 123456                                                                                                                                                                       |
| `owner`                                                                                                                                                                      | *string*                                                                                                                                                                     | :heavy_check_mark:                                                                                                                                                           | Blockchain address in Union format `${blockchainGroup}:${token}`                                                                                                             | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                                                                                                          |
| `value`                                                                                                                                                                      | *string*                                                                                                                                                                     | :heavy_check_mark:                                                                                                                                                           | N/A                                                                                                                                                                          | 123456                                                                                                                                                                       |
| `source`                                                                                                                                                                     | [models.OwnershipSource](../models/ownershipsource.md)                                                                                                                       | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          |                                                                                                                                                                              |
| `createdAt`                                                                                                                                                                  | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)                                                                                | :heavy_check_mark:                                                                                                                                                           | N/A                                                                                                                                                                          |                                                                                                                                                                              |
| `lastUpdatedAt`                                                                                                                                                              | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)                                                                                | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          |                                                                                                                                                                              |
| ~~`creators`~~                                                                                                                                                               | [models.Creator](../models/creator.md)[]                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                           | : warning: ** DEPRECATED **: This will be removed in a future release, please migrate away from it as soon as possible.<br/><br/>Creators of the target item                 |                                                                                                                                                                              |
| `lazyValue`                                                                                                                                                                  | *string*                                                                                                                                                                     | :heavy_check_mark:                                                                                                                                                           | N/A                                                                                                                                                                          | 123456                                                                                                                                                                       |
| `pending`                                                                                                                                                                    | *models.ItemHistory*[]                                                                                                                                                       | :heavy_check_mark:                                                                                                                                                           | Pending information about the item                                                                                                                                           |                                                                                                                                                                              |
| `bestSellOrder`                                                                                                                                                              | [models.Order](../models/order.md)                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          |                                                                                                                                                                              |
| `originOrders`                                                                                                                                                               | [models.OriginOrders](../models/originorders.md)[]                                                                                                                           | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          |                                                                                                                                                                              |
| `version`                                                                                                                                                                    | *number*                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          |                                                                                                                                                                              |