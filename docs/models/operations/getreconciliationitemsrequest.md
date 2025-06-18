# GetReconciliationItemsRequest

## Example Usage

```typescript
import { GetReconciliationItemsRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetReconciliationItemsRequest = {
  blockchain: "ETHEREUM",
  updatedAfterInclusive: new Date("2024-12-05T01:03:00.475Z"),
  updatedBeforeExclusive: new Date("2024-08-04T01:56:35.002Z"),
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `blockchain`                                                                                  | [models.Blockchain](../../models/blockchain.md)                                               | :heavy_check_mark:                                                                            | Blockchain name                                                                               | ETHEREUM                                                                                      |
| `updatedAfterInclusive`                                                                       | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | Only items with lastUpdatedAt after (inclusive) will be returned                              |                                                                                               |
| `updatedBeforeExclusive`                                                                      | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | Only items with lastUpdatedAt before (exclusive) will be returned                             |                                                                                               |
| `continuation`                                                                                | *string*                                                                                      | :heavy_minus_sign:                                                                            | Paging cursor                                                                                 |                                                                                               |
| `size`                                                                                        | *number*                                                                                      | :heavy_minus_sign:                                                                            | The maximum number of results to be returned. If not specified, a predefined number is used.  |                                                                                               |