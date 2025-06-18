# SolanaNftAssetType

## Example Usage

```typescript
import { SolanaNftAssetType } from "@rarible/protocol-mcp";

let value: SolanaNftAssetType = {
  atType: "SOLANA_NFT",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
};
```

## Fields

| Field                                                                                                                             | Type                                                                                                                              | Required                                                                                                                          | Description                                                                                                                       | Example                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `atType`                                                                                                                          | [models.SolanaNftAssetTypeAtType](../models/solananftassettypeattype.md)                                                          | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `contract`                                                                                                                        | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | Blockchain contract address in Union format `ETHEREUM:${token}`                                                                   | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                                                                               |
| `collection`                                                                                                                      | *string*                                                                                                                          | :heavy_minus_sign:                                                                                                                | Collection id                                                                                                                     | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                                                               |
| `itemId`                                                                                                                          | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | Item Id, has format `ETHEREUM:${token}:${tokenId}`                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410 |