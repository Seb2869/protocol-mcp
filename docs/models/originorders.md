# OriginOrders

## Example Usage

```typescript
import { OriginOrders } from "@rarible/protocol-mcp";

let value: OriginOrders = {
  origin: "<value>",
  bestSellOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "OBJKT",
    status: "FILLED",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2024-01-29T03:49:57.798Z"),
    lastUpdatedAt: new Date("2024-10-22T03:34:04.542Z"),
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
      atType: "ETH_OPEN_SEA_V1",
      exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      makerRelayerFee: "123456",
      takerRelayerFee: "123456",
      makerProtocolFee: "123456",
      takerProtocolFee: "123456",
      feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      feeMethod: "PROTOCOL_FEE",
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
  bestBidOrder: {
    id:
      "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    fill: "123456.789",
    platform: "FXHASH",
    status: "ACTIVE",
    makeStock: "123456.789",
    cancelled: false,
    createdAt: new Date("2025-01-02T01:00:08.649Z"),
    lastUpdatedAt: new Date("2023-06-04T07:51:41.164Z"),
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
        uri: "https://nimble-adaptation.name/",
        supply: "123456",
        creators: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 261613,
          },
        ],
        royalties: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 321945,
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
      atType: "ETH_RARIBLE_V2_DATA_V3_SELL",
      payout: {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 614152,
      },
      originFeeFirst: {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 137681,
      },
      originFeeSecond: {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 853751,
      },
      maxFeesBasePoint: 110424,
    },
  },
};
```

## Fields

| Field                              | Type                               | Required                           | Description                        |
| ---------------------------------- | ---------------------------------- | ---------------------------------- | ---------------------------------- |
| `origin`                           | *string*                           | :heavy_check_mark:                 | N/A                                |
| `bestSellOrder`                    | [models.Order](../models/order.md) | :heavy_minus_sign:                 | N/A                                |
| `bestBidOrder`                     | [models.Order](../models/order.md) | :heavy_minus_sign:                 | N/A                                |