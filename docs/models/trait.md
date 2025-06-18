# Trait

Combination of Item attribute key with list of values

## Example Usage

```typescript
import { Trait } from "@rarible/protocol-mcp";

let value: Trait = {
  key: {
    value: "<value>",
    count: 230944,
  },
  values: [
    {
      value: "<value>",
      count: 972446,
    },
  ],
};
```

## Fields

| Field                                                   | Type                                                    | Required                                                | Description                                             |
| ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| `key`                                                   | [models.TraitEntry](../models/traitentry.md)            | :heavy_check_mark:                                      | Combination of Item attribute key/value with it's count |
| `values`                                                | [models.TraitEntry](../models/traitentry.md)[]          | :heavy_check_mark:                                      | N/A                                                     |