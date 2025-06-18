# SalesChart

## Example Usage

```typescript
import { SalesChart } from "@rarible/protocol-mcp";

let value: SalesChart = {
  dates: [
    new Date("2023-05-09T06:36:51.943Z"),
  ],
  pricesNative: [
    "123456.789",
  ],
  itemIds: [
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  ],
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `cursor`                                                                                        | *string*                                                                                        | :heavy_minus_sign:                                                                              | Combined continuation token to paginate search result                                           |
| `dates`                                                                                         | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)[] | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `pricesNative`                                                                                  | *string*[]                                                                                      | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `itemIds`                                                                                       | *string*[]                                                                                      | :heavy_check_mark:                                                                              | N/A                                                                                             |