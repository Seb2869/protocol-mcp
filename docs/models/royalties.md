# Royalties

## Example Usage

```typescript
import { Royalties } from "@rarible/protocol-mcp";

let value: Royalties = {
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 685342,
    },
  ],
};
```

## Fields

| Field                                    | Type                                     | Required                                 | Description                              |
| ---------------------------------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| `royalties`                              | [models.Royalty](../models/royalty.md)[] | :heavy_check_mark:                       | N/A                                      |