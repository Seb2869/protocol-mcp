# OlapPriceWithUsd

## Example Usage

```typescript
import { OlapPriceWithUsd } from "@rarible/protocol-mcp";

let value: OlapPriceWithUsd = {
  currency: "Netherlands Antillian Guilder",
  value: 8835.21,
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `currency`         | *string*           | :heavy_check_mark: | N/A                |
| `value`            | *number*           | :heavy_check_mark: | Amount of currency |
| `valueUsd`         | *number*           | :heavy_minus_sign: | Amount in USD      |