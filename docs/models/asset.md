# Asset

## Example Usage

```typescript
import { Asset } from "@rarible/protocol-mcp";

let value: Asset = {
  type: {
    atType: "CURRENCY_TOKEN",
    contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  },
  value: "123456.789",
};
```

## Fields

| Field              | Type               | Required           | Description        | Example            |
| ------------------ | ------------------ | ------------------ | ------------------ | ------------------ |
| `type`             | *models.AssetType* | :heavy_check_mark: | N/A                |                    |
| `value`            | *string*           | :heavy_check_mark: | N/A                | 123456.789         |