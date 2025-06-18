# AssetType


## Supported Types

### `models.NativeCurrencyAssetType`

```typescript
const value: models.NativeCurrencyAssetType = {
  blockchain: "ETHEREUM",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  atType: "CURRENCY_NATIVE",
};
```

### `models.TokenCurrencyAssetType`

```typescript
const value: models.TokenCurrencyAssetType = {
  atType: "CURRENCY_TOKEN",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

### `models.NftAssetType`

```typescript
const value: models.NftAssetType = {
  atType: "NFT",
  collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
};
```

### `models.NftOfCollectionAssetType`

```typescript
const value: models.NftOfCollectionAssetType = {
  atType: "NFT_OF_COLLECTION",
  collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
};
```

### `models.FlowAssetTypeNft`

```typescript
const value: models.FlowAssetTypeNft = {
  atType: "FLOW_NFT",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
};
```

### `models.FlowAssetTypeFt`

```typescript
const value: models.FlowAssetTypeFt = {
  atType: "FLOW_FT",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

### `models.EthEthereumAssetType`

```typescript
const value: models.EthEthereumAssetType = {
  atType: "ETH",
  blockchain: "ETHEREUM",
};
```

### `models.EthErc20AssetType`

```typescript
const value: models.EthErc20AssetType = {
  atType: "ERC20",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

### `models.EthErc721AssetType`

```typescript
const value: models.EthErc721AssetType = {
  atType: "ERC721",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
};
```

### `models.EthErc721LazyAssetType`

```typescript
const value: models.EthErc721LazyAssetType = {
  atType: "ERC721_Lazy",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
  uri: "https://pessimistic-decryption.com/",
  creators: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 469575,
    },
  ],
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 41800,
    },
  ],
  signatures: [
    "<value>",
  ],
};
```

### `models.EthErc1155AssetType`

```typescript
const value: models.EthErc1155AssetType = {
  atType: "ERC1155",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
};
```

### `models.EthErc1155LazyAssetType`

```typescript
const value: models.EthErc1155LazyAssetType = {
  atType: "ERC1155_Lazy",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
  uri: "https://useless-approach.info/",
  supply: "123456",
  creators: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 508819,
    },
  ],
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 92369,
    },
  ],
  signatures: [
    "<value>",
  ],
};
```

### `models.EthCryptoPunksAssetType`

```typescript
const value: models.EthCryptoPunksAssetType = {
  atType: "CRYPTO_PUNKS",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: 882070,
};
```

### `models.EthGenerativeArtAssetType`

```typescript
const value: models.EthGenerativeArtAssetType = {
  atType: "GEN_ART",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
};
```

### `models.EthCollectionAssetType`

```typescript
const value: models.EthCollectionAssetType = {
  atType: "COLLECTION",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
};
```

### `models.SolanaNftAssetType`

```typescript
const value: models.SolanaNftAssetType = {
  atType: "SOLANA_NFT",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
};
```

### `models.SolanaFtAssetType`

```typescript
const value: models.SolanaFtAssetType = {
  atType: "SOLANA_FT",
  address: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
};
```

### `models.SolanaSolAssetType`

```typescript
const value: models.SolanaSolAssetType = {
  atType: "SOLANA_SOL",
};
```

