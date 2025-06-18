# OrderMatchActivity


## Supported Types

### `models.OrderMatchSwap`

```typescript
const value: models.OrderMatchSwap = {
  left: {
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    asset: {
      type: {
        atType: "ERC721_Lazy",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        tokenId: "123456",
        uri: "https://sturdy-mentor.biz/",
        creators: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 956930,
          },
        ],
        royalties: [
          {
            account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
            value: 844922,
          },
        ],
        signatures: [
          "<value>",
        ],
      },
      value: "123456.789",
    },
  },
  right: {
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    asset: {
      type: {
        atType: "NFT",
        collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        itemId:
          "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
      },
      value: "123456.789",
    },
  },
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  source: "SUDOSWAP",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2023-06-24T10:07:05.154Z"),
};
```

### `models.OrderMatchSell`

```typescript
const value: models.OrderMatchSell = {
  nft: {
    type: {
      atType: "ETH",
      blockchain: "ETHEREUM",
    },
    value: "123456.789",
  },
  payment: {
    type: {
      atType: "CURRENCY_TOKEN",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456.789",
  },
  buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  price: "123456.789",
  priceUsd: "123456.789",
  amountUsd: "123456.789",
  type: "SELL",
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  source: "IMMUTABLEX",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2024-09-19T05:34:16.255Z"),
};
```

