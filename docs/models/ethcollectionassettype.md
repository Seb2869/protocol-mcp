# EthCollectionAssetType

## Example Usage

```typescript
import { EthCollectionAssetType } from "@rarible/protocol-mcp";

let value: EthCollectionAssetType = {
  atType: "COLLECTION",
  contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      | Example                                                                          |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `atType`                                                                         | [models.EthCollectionAssetTypeAtType](../models/ethcollectionassettypeattype.md) | :heavy_check_mark:                                                               | N/A                                                                              |                                                                                  |
| `contract`                                                                       | *string*                                                                         | :heavy_check_mark:                                                               | Blockchain contract address in Union format `ETHEREUM:${token}`                  | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430                              |
| `collection`                                                                     | *string*                                                                         | :heavy_minus_sign:                                                               | Collection id                                                                    | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                              |