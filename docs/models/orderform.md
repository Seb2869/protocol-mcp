# OrderForm


## Supported Types

### `models.EthRaribleOrderForm`

```typescript
const value: models.EthRaribleOrderForm = {
  data: {
    atType: "ETH_RARIBLE_V2_3",
    payouts: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 540502,
      },
    ],
    originFees: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 260506,
      },
    ],
    isMakeFill: false,
  },
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    assetType: {
      blockchain: "ETHEREUM",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      atType: "CURRENCY_NATIVE",
    },
    value: "123456",
  },
  take: {
    assetType: {
      atType: "ERC20",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456",
  },
  endedAt: new Date("2023-04-15T03:36:37.387Z"),
  salt: "123456",
  signature: "<value>",
  blockchain: "ETHEREUM",
};
```

