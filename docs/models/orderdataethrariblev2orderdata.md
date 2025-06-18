# OrderDataEthRaribleV2OrderData


## Supported Types

### `models.EthOrderDataRaribleV2DataV1`

```typescript
const value: models.EthOrderDataRaribleV2DataV1 = {
  atType: "ETH_RARIBLE_V2",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 7981,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 45075,
    },
  ],
};
```

### `models.EthOrderDataRaribleV2DataV2`

```typescript
const value: models.EthOrderDataRaribleV2DataV2 = {
  atType: "ETH_RARIBLE_V2_2",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 213054,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 390932,
    },
  ],
  isMakeFill: false,
};
```

### `models.EthOrderDataRaribleV2DataV3`

```typescript
const value: models.EthOrderDataRaribleV2DataV3 = {
  atType: "ETH_RARIBLE_V2_3",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 339435,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 461452,
    },
  ],
  isMakeFill: false,
};
```

### `models.EthOrderDataRaribleV2DataV3Sell`

```typescript
const value: models.EthOrderDataRaribleV2DataV3Sell = {
  atType: "ETH_RARIBLE_V2_DATA_V3_SELL",
  payout: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 569433,
  },
  originFeeFirst: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 685026,
  },
  originFeeSecond: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 402141,
  },
  maxFeesBasePoint: 290634,
};
```

### `models.EthOrderDataRaribleV2DataV3Buy`

```typescript
const value: models.EthOrderDataRaribleV2DataV3Buy = {
  atType: "ETH_RARIBLE_V2_DATA_V3_BUY",
  payout: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 964229,
  },
  originFeeFirst: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 418795,
  },
  originFeeSecond: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 513879,
  },
};
```

