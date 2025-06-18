# EthOrderFormAsset

## Example Usage

```typescript
import { EthOrderFormAsset } from "@rarible/protocol-mcp";

let value: EthOrderFormAsset = {
  assetType: {
    atType: "FLOW_FT",
    contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  },
  value: "123456",
};
```

## Fields

| Field              | Type               | Required           | Description        | Example            |
| ------------------ | ------------------ | ------------------ | ------------------ | ------------------ |
| `assetType`        | *models.AssetType* | :heavy_check_mark: | N/A                |                    |
| `value`            | *string*           | :heavy_check_mark: | N/A                | 123456             |