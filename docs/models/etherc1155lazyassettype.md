# EthErc1155LazyAssetType

## Example Usage

```typescript
import { EthErc1155LazyAssetType } from "@rarible/protocol-mcp";

let value: EthErc1155LazyAssetType = {
  atType: "ERC1155_Lazy",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
  uri: "https://scented-loaf.net",
  supply: "123456",
  creators: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 713692,
    },
  ],
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 950797,
    },
  ],
  signatures: [
    "<value>",
  ],
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        | Example                                                                            |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `atType`                                                                           | [models.EthErc1155LazyAssetTypeAtType](../models/etherc1155lazyassettypeattype.md) | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `contract`                                                                         | *string*                                                                           | :heavy_check_mark:                                                                 | Blockchain contract address in Union format `ETHEREUM:${token}`                    | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                |
| `collection`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Collection id                                                                      | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                |
| `tokenId`                                                                          | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |
| `uri`                                                                              | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `supply`                                                                           | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |
| `creators`                                                                         | [models.Creator](../models/creator.md)[]                                           | :heavy_check_mark:                                                                 | Creators of the target item                                                        |                                                                                    |
| `royalties`                                                                        | [models.Royalty](../models/royalty.md)[]                                           | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `signatures`                                                                       | *string*[]                                                                         | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |