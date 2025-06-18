# NftAssetType

## Example Usage

```typescript
import { NftAssetType } from "@rarible/protocol-mcp";

let value: NftAssetType = {
  atType: "NFT",
  collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  itemId:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
};
```

## Fields

| Field                                                                                                                             | Type                                                                                                                              | Required                                                                                                                          | Description                                                                                                                       | Example                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `atType`                                                                                                                          | [models.NftAssetTypeAtType](../models/nftassettypeattype.md)                                                                      | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `collectionId`                                                                                                                    | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | Collection id                                                                                                                     | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                                                               |
| `itemId`                                                                                                                          | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | Item Id, has format `ETHEREUM:${token}:${tokenId}`                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410 |
| `standard`                                                                                                                        | [models.Standard](../models/standard.md)                                                                                          | :heavy_minus_sign:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |