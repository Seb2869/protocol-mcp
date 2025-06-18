# ItemCollection

## Example Usage

```typescript
import { ItemCollection } from "@rarible/protocol-mcp";

let value: ItemCollection = {
  id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  name: "<value>",
  bestBidOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "VERSUM",
    status: "FILLED",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2024-02-04T12:03:54.063Z"),
    lastUpdatedAt: new Date("2023-11-30T00:06:37.333Z"),
    makePrice: "123456.789",
    takePrice: "123456.789",
    makePriceUsd: "123456.789",
    takePriceUsd: "123456.789",
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    make: {
      type: {
        atType: "ERC1155",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        tokenId: "123456",
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
      atType: "RAW",
    },
  },
  bestSellOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "OBJKT",
    status: "CANCELLED",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2023-11-14T23:03:55.977Z"),
    lastUpdatedAt: new Date("2025-02-17T18:10:15.598Z"),
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
        uri: "https://portly-excess.com",
        supply: "123456",
        creators: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 693556,
          },
        ],
        royalties: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 228518,
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
        atType: "SOLANA_SOL",
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
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `id`                                                | *string*                                            | :heavy_check_mark:                                  | Collection id                                       | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8 |
| `name`                                              | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |                                                     |
| `bestBidOrder`                                      | [models.Order](../models/order.md)                  | :heavy_minus_sign:                                  | N/A                                                 |                                                     |
| `bestSellOrder`                                     | [models.Order](../models/order.md)                  | :heavy_minus_sign:                                  | N/A                                                 |                                                     |