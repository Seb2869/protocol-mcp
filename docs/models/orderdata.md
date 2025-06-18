# OrderData


## Supported Types

### `models.RawOrderData`

```typescript
const value: models.RawOrderData = {
  atType: "RAW",
};
```

### `models.EthOrderDataLegacy`

```typescript
const value: models.EthOrderDataLegacy = {
  atType: "ETH_RARIBLE_V1",
  fee: "123456",
};
```

### `models.OrderDataEthRaribleV2OrderData`

```typescript
const value: models.OrderDataEthRaribleV2OrderData = {
  atType: "ETH_RARIBLE_V2_DATA_V3_BUY",
  payout: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 273073,
  },
  originFeeFirst: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 627094,
  },
  originFeeSecond: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 271628,
  },
};
```

### `models.EthOrderOpenSeaV1DataV1`

```typescript
const value: models.EthOrderOpenSeaV1DataV1 = {
  atType: "ETH_OPEN_SEA_V1",
  exchange: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  makerRelayerFee: "123456",
  takerRelayerFee: "123456",
  makerProtocolFee: "123456",
  takerProtocolFee: "123456",
  feeRecipient: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  feeMethod: "SPLIT_FEE",
  side: "SELL",
  saleKind: "DUTCH_AUCTION",
  howToCall: "CALL",
  callData: "<value>",
  replacementPattern: "<value>",
  staticTarget: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  staticExtraData: "<value>",
  extra: "123456",
};
```

### `models.EthOrderSeaportDataV1`

```typescript
const value: models.EthOrderSeaportDataV1 = {
  atType: "ETH_BASIC_SEAPORT_DATA_V1",
  protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  orderType: "PARTIAL_RESTRICTED",
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
      itemType: "ERC721",
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
};
```

### `models.EthOrderCryptoPunksData`

```typescript
const value: models.EthOrderCryptoPunksData = {
  atType: "ETH_CRYPTO_PUNKS",
};
```

### `models.FlowOrderDataV1`

```typescript
const value: models.FlowOrderDataV1 = {
  atType: "FLOW_RARIBLE_V1",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 438041,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 80636,
    },
  ],
};
```

### `models.SolanaAuctionHouseDataV1`

```typescript
const value: models.SolanaAuctionHouseDataV1 = {
  atType: "SOLANA_AUCTION_HOUSE_V1",
  auctionHouse: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

### `models.ImmutablexOrderDataV1`

```typescript
const value: models.ImmutablexOrderDataV1 = {
  atType: "IMMUTABLEX_RARIBLE_V1",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 255058,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 658372,
    },
  ],
};
```

