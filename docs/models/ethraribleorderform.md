# EthRaribleOrderForm


## Supported Types

### `models.EthRaribleV2OrderForm`

```typescript
const value: models.EthRaribleV2OrderForm = {
  data: {
    atType: "ETH_RARIBLE_V2_2",
    payouts: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 921675,
      },
    ],
    originFees: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 521748,
      },
    ],
    isMakeFill: false,
  },
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    assetType: {
      atType: "SOLANA_NFT",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      itemId:
        "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
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
  endedAt: new Date("2023-10-07T20:47:03.395Z"),
  salt: "123456",
  signature: "<value>",
  blockchain: "ETHEREUM",
};
```

