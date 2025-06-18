# OrderIds

## Example Usage

```typescript
import { OrderIds } from "@rarible/protocol-mcp";

let value: OrderIds = {
  ids: [
    "<value>",
  ],
};
```

## Fields

| Field                                              | Type                                               | Required                                           | Description                                        |
| -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- |
| `ids`                                              | *string*[]                                         | :heavy_check_mark:                                 | Array of the orders Ids in format 'ETHEREUM:${id}' |