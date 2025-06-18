# ExtendedTraitProperties

## Example Usage

```typescript
import { ExtendedTraitProperties } from "@rarible/protocol-mcp";

let value: ExtendedTraitProperties = {
  traits: [
    {
      key: "<key>",
      value: "<value>",
      rarity: 5570.98,
    },
  ],
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `continuation`                                                       | *string*                                                             | :heavy_minus_sign:                                                   | Continuation token to paginate result                                |
| `traits`                                                             | [models.ExtendedTraitProperty](../models/extendedtraitproperty.md)[] | :heavy_check_mark:                                                   | List of ExtendedTraitProperty                                        |