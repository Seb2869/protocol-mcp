# ReconciliationEntity

## Example Usage

```typescript
import { ReconciliationEntity } from "@rarible/protocol-mcp";

let value: ReconciliationEntity = {
  id: "<id>",
  version: 3,
  lastUpdatedAt: new Date("2023-10-25T13:14:13.487Z"),
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `id`                                                                                          | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `version`                                                                                     | *number*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `lastUpdatedAt`                                                                               | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `deleted`                                                                                     | *boolean*                                                                                     | :heavy_minus_sign:                                                                            | N/A                                                                                           |