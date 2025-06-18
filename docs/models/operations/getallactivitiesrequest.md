# GetAllActivitiesRequest

## Example Usage

```typescript
import { GetAllActivitiesRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetAllActivitiesRequest = {
  blockchains: [
    "ETHEREUM",
  ],
  type: [
    "BRIDGE_TO",
  ],
  bidCurrencies: [
    "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  ],
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `blockchains`                                                                                     | [models.Blockchain](../../models/blockchain.md)[]                                                 | :heavy_minus_sign:                                                                                | Names of the blockchain networks. If no one specified, data from all blockchains will be returned |
| `type`                                                                                            | [models.ActivityType](../../models/activitytype.md)[]                                             | :heavy_check_mark:                                                                                | Activity type                                                                                     |
| `bidCurrencies`                                                                                   | *string*[]                                                                                        | :heavy_minus_sign:                                                                                | Currency for BID and CANCEL_BID activity types                                                    |
| `continuation`                                                                                    | *string*                                                                                          | :heavy_minus_sign:                                                                                | Continuation token from the previous response                                                     |
| `cursor`                                                                                          | *string*                                                                                          | :heavy_minus_sign:                                                                                | Combined continuation token from the previous response                                            |
| `size`                                                                                            | *number*                                                                                          | :heavy_minus_sign:                                                                                | The number of items to return                                                                     |
| `sort`                                                                                            | [models.ActivitySort](../../models/activitysort.md)                                               | :heavy_minus_sign:                                                                                | Sorting by data update time                                                                       |