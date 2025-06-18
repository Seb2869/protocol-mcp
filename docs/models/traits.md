# Traits

## Example Usage

```typescript
import { Traits } from "@rarible/protocol-mcp";

let value: Traits = {
  traits: [
    {
      key: {
        value: "<value>",
        count: 411843,
      },
      values: [
        {
          value: "<value>",
          count: 528775,
        },
      ],
    },
  ],
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `continuation`                                      | *string*                                            | :heavy_minus_sign:                                  | Continuation token to paginate traits search result |
| `traits`                                            | [models.Trait](../models/trait.md)[]                | :heavy_check_mark:                                  | List of found traits                                |