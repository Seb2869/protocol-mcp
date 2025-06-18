# GetValidatedOrderByIdRequest

## Example Usage

```typescript
import { GetValidatedOrderByIdRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetValidatedOrderByIdRequest = {
  id:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 | Example                                                                     |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `id`                                                                        | *string*                                                                    | :heavy_check_mark:                                                          | Order Id, has format 'ETHEREUM:${id}'                                       | ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143 |