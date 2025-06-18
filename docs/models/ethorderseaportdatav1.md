# EthOrderSeaportDataV1


## Supported Types

### `models.EthOrderBasicSeaportDataV1`

```typescript
const value: models.EthOrderBasicSeaportDataV1 = {
  atType: "ETH_BASIC_SEAPORT_DATA_V1",
  protocol: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  orderType: "PARTIAL_OPEN",
  offer: [
    {
      itemType: "NATIVE",
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
};
```

