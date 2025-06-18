# EthErc721AssetType

## Example Usage

```typescript
import { EthErc721AssetType } from "@rarible/protocol-mcp";

let value: EthErc721AssetType = {
  atType: "ERC721",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  tokenId: "123456",
};
```

## Fields

| Field                                                                    | Type                                                                     | Required                                                                 | Description                                                              | Example                                                                  |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `atType`                                                                 | [models.EthErc721AssetTypeAtType](../models/etherc721assettypeattype.md) | :heavy_check_mark:                                                       | N/A                                                                      |                                                                          |
| `contract`                                                               | *string*                                                                 | :heavy_check_mark:                                                       | Blockchain contract address in Union format `ETHEREUM:${token}`          | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                      |
| `collection`                                                             | *string*                                                                 | :heavy_minus_sign:                                                       | Collection id                                                            | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                      |
| `tokenId`                                                                | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      | 123456                                                                   |