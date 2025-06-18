# Orders

## Example Usage

```typescript
import { Orders } from "@rarible/protocol-mcp";

let value: Orders = {
  orders: [
    {
      id:
        "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
      fill: "123456.789",
      platform: "FXHASH",
      status: "FILLED",
      makeStock: "123456.789",
      cancelled: false,
      createdAt: new Date("2023-07-13T19:05:16.033Z"),
      lastUpdatedAt: new Date("2025-10-22T00:16:28.547Z"),
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
          collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
          tokenId: "123456",
          uri: "https://humiliating-finding.org/",
          creators: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 989962,
            },
          ],
          royalties: [
            {
              account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
              value: 534663,
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
        atType: "ETH_RARIBLE_V2_3",
        payouts: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 110961,
          },
        ],
        originFees: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 571008,
          },
        ],
        isMakeFill: false,
      },
    },
  ],
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `continuation`                                      | *string*                                            | :heavy_minus_sign:                                  | Continuation token to paginate orders search result |
| `orders`                                            | [models.Order](../models/order.md)[]                | :heavy_check_mark:                                  | List of found orders                                |