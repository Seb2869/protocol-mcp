# TraitSort

Used when the search sort is set as TRAIT

## Example Usage

```typescript
import { TraitSort } from "@rarible/protocol-mcp";

let value: TraitSort = {
  key: "hat",
};
```

## Fields

| Field                                      | Type                                       | Required                                   | Description                                | Example                                    |
| ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| `key`                                      | *string*                                   | :heavy_check_mark:                         | Trait key                                  | hat                                        |
| `order`                                    | [models.SortOrder](../models/sortorder.md) | :heavy_minus_sign:                         | N/A                                        |                                            |
| `type`                                     | [models.SortType](../models/sorttype.md)   | :heavy_minus_sign:                         | N/A                                        |                                            |