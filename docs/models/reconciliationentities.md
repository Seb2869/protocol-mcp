# ReconciliationEntities

## Example Usage

```typescript
import { ReconciliationEntities } from "@rarible/protocol-mcp";

let value: ReconciliationEntities = {
  entities: [
    {
      id: "<id>",
      version: 7,
      lastUpdatedAt: new Date("2023-04-05T05:38:10.559Z"),
    },
  ],
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `entities`                                                         | [models.ReconciliationEntity](../models/reconciliationentity.md)[] | :heavy_check_mark:                                                 | N/A                                                                |
| `continuation`                                                     | *string*                                                           | :heavy_minus_sign:                                                 | N/A                                                                |