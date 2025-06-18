# GetUsdRateRequest

## Example Usage

```typescript
import { GetUsdRateRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetUsdRateRequest = {
  currencyId: "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  at: new Date("2022-01-01T12:00:00Z"),
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `currencyId`                                                                                  | *string*                                                                                      | :heavy_check_mark:                                                                            | Currency Id, has format `ETHEREUM:${token}` or `ETHEREUM:${token}:${tokenId}`                 | ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2                                           |
| `at`                                                                                          | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | Date and time for getting currency USD rate (if not specified, returns actual rate)           | 2022-01-01T12:00:00Z                                                                          |