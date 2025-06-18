# ActivityUserFilter

## Example Usage

```typescript
import { ActivityUserFilter } from "@rarible/protocol-mcp";

let value: ActivityUserFilter = {
  any: [
    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  ],
  from: [
    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  ],
  to: [
    "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  ],
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `any`              | *string*[]         | :heavy_minus_sign: | N/A                |
| `from`             | *string*[]         | :heavy_minus_sign: | N/A                |
| `to`               | *string*[]         | :heavy_minus_sign: | N/A                |