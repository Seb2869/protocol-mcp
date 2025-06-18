# EthRaribleV2OrderForm

## Example Usage

```typescript
import { EthRaribleV2OrderForm } from "@rarible/protocol-mcp";

let value: EthRaribleV2OrderForm = {
  data: {
    atType: "ETH_RARIBLE_V2_3",
    payouts: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 298208,
      },
    ],
    originFees: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 1632,
      },
    ],
    isMakeFill: false,
  },
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    assetType: {
      atType: "SOLANA_FT",
      address: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456",
  },
  take: {
    assetType: {
      atType: "FLOW_FT",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456",
  },
  endedAt: new Date("2024-01-08T15:25:50.284Z"),
  salt: "123456",
  signature: "<value>",
  blockchain: "ETHEREUM",
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `atType`                                                                                      | [models.OrderFormAtType](../models/orderformattype.md)                                        | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |
| `data`                                                                                        | *models.EthRaribleV2OrderData*                                                                | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `maker`                                                                                       | *string*                                                                                      | :heavy_check_mark:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `taker`                                                                                       | *string*                                                                                      | :heavy_minus_sign:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `make`                                                                                        | [models.EthOrderFormAsset](../models/ethorderformasset.md)                                    | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `take`                                                                                        | [models.EthOrderFormAsset](../models/ethorderformasset.md)                                    | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `startedAt`                                                                                   | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |
| `endedAt`                                                                                     | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `salt`                                                                                        | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | 123456                                                                                        |
| `signature`                                                                                   | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `blockchain`                                                                                  | [models.Blockchain](../models/blockchain.md)                                                  | :heavy_check_mark:                                                                            | N/A                                                                                           | ETHEREUM                                                                                      |