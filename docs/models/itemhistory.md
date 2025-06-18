# ItemHistory

History of item


## Supported Types

### `models.ItemRoyalty`

```typescript
const value: models.ItemRoyalty = {
  atType: "ROYALTY",
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 672733,
    },
  ],
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  tokenId: "123456",
  value: "123456",
  date: new Date("2023-12-25T03:53:43.864Z"),
};
```

### `models.ItemHistoryItemTransfer`

```typescript
const value: models.ItemHistoryItemTransfer = {
  atType: "TRANSFER",
  from: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  tokenId: "123456",
  value: "123456",
  date: new Date("2025-08-12T08:33:43.095Z"),
};
```

