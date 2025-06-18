# Activity


## Supported Types

### `models.MintActivity`

```typescript
const value: models.MintActivity = {
  atType: "MINT",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  value: "123456",
  mintPrice: "123456.789",
  mintPayment: {
    type: {
      atType: "ERC1155_Lazy",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      tokenId: "123456",
      uri: "https://blind-ostrich.biz",
      supply: "123456",
      creators: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 55594,
        },
      ],
      royalties: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 447686,
        },
      ],
      signatures: [
        "<value>",
      ],
    },
    value: "123456.789",
  },
  mintPriceUsd: "123456.789",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2023-11-22T09:48:12.896Z"),
};
```

### `models.BurnActivity`

```typescript
const value: models.BurnActivity = {
  atType: "BURN",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  value: "123456",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2025-08-08T02:48:24.257Z"),
};
```

### `models.TransferActivity`

```typescript
const value: models.TransferActivity = {
  atType: "TRANSFER",
  from: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  value: "123456",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2025-02-21T20:18:47.476Z"),
};
```

### `models.SendToChainActivity`

```typescript
const value: models.SendToChainActivity = {
  atType: "SEND_TO_CHAIN",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  to: "<value>",
  chainId: "123456",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  value: "123456",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2023-07-25T07:55:09.567Z"),
};
```

### `models.ReceiveFromChainActivity`

```typescript
const value: models.ReceiveFromChainActivity = {
  atType: "RECEIVE_FROM_CHAIN",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  from: "<value>",
  chainId: "123456",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  value: "123456",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2025-07-04T16:28:06.108Z"),
};
```

### `models.OrderMatchActivity`

```typescript
const value: models.OrderMatchActivity = {
  nft: {
    type: {
      atType: "SOLANA_FT",
      address: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456.789",
  },
  payment: {
    type: {
      atType: "FLOW_NFT",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      tokenId: "123456",
    },
    value: "123456.789",
  },
  buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  price: "123456.789",
  priceUsd: "123456.789",
  amountUsd: "123456.789",
  type: "ACCEPT_BID",
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  source: "TOPAZ",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2023-05-11T11:03:14.943Z"),
};
```

### `models.OrderBidActivity`

```typescript
const value: models.OrderBidActivity = {
  atType: "BID",
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  hash: "<value>",
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    type: {
      atType: "FLOW_NFT",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      tokenId: "123456",
    },
    value: "123456.789",
  },
  take: {
    type: {
      atType: "ERC721",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      tokenId: "123456",
    },
    value: "123456.789",
  },
  price: "123456.789",
  priceUsd: "123456.789",
  id: "ETHEREUM:${id}",
  date: new Date("2023-12-08T17:11:21.163Z"),
};
```

### `models.OrderListActivity`

```typescript
const value: models.OrderListActivity = {
  atType: "LIST",
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  hash: "<value>",
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    type: {
      atType: "ERC20",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456.789",
  },
  take: {
    type: {
      atType: "COLLECTION",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    },
    value: "123456.789",
  },
  price: "123456.789",
  priceUsd: "123456.789",
  id: "ETHEREUM:${id}",
  date: new Date("2024-03-29T23:10:28.709Z"),
};
```

### `models.OrderCancelBidActivity`

```typescript
const value: models.OrderCancelBidActivity = {
  atType: "CANCEL_BID",
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  hash: "<value>",
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    atType: "ERC1155_Lazy",
    contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    tokenId: "123456",
    uri: "https://homely-bidet.info/",
    supply: "123456",
    creators: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 309259,
      },
    ],
    royalties: [
      {
        account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
        value: 482516,
      },
    ],
    signatures: [
      "<value>",
    ],
  },
  take: {
    atType: "SOLANA_NFT",
    contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    itemId:
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  },
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2023-11-16T22:54:03.667Z"),
};
```

### `models.OrderCancelListActivity`

```typescript
const value: models.OrderCancelListActivity = {
  atType: "CANCEL_LIST",
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  hash: "<value>",
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    atType: "SOLANA_FT",
    address: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  },
  take: {
    atType: "FLOW_NFT",
    contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    tokenId: "123456",
  },
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2023-06-08T19:27:27.890Z"),
};
```

### `models.L2DepositActivity`

```typescript
const value: models.L2DepositActivity = {
  atType: "L2_DEPOSIT",
  user: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  status: "<value>",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  value: "123456",
  id: "ETHEREUM:${id}",
  date: new Date("2023-10-04T21:38:48.811Z"),
};
```

### `models.L2WithdrawalActivity`

```typescript
const value: models.L2WithdrawalActivity = {
  atType: "L2_WITHDRAWAL",
  user: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  status: "<value>",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  value: "123456",
  id: "ETHEREUM:${id}",
  date: new Date("2024-09-08T18:27:07.667Z"),
};
```

