# HtmlContent

## Example Usage

```typescript
import { HtmlContent } from "@rarible/protocol-mcp";

let value: HtmlContent = {
  url: "https://probable-embarrassment.org",
  representation: "ORIGINAL",
  mimeType: "image/png",
};
```

## Fields

| Field                                                        | Type                                                         | Required                                                     | Description                                                  | Example                                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `atType`                                                     | [models.AtTypeHTML](../models/attypehtml.md)                 | :heavy_minus_sign:                                           | N/A                                                          |                                                              |
| `fileName`                                                   | *string*                                                     | :heavy_minus_sign:                                           | N/A                                                          |                                                              |
| `url`                                                        | *string*                                                     | :heavy_check_mark:                                           | N/A                                                          |                                                              |
| `representation`                                             | [models.RepresentationHTML](../models/representationhtml.md) | :heavy_check_mark:                                           | N/A                                                          |                                                              |
| `mimeType`                                                   | *string*                                                     | :heavy_minus_sign:                                           | N/A                                                          | image/png                                                    |
| `size`                                                       | *number*                                                     | :heavy_minus_sign:                                           | N/A                                                          |                                                              |
| `available`                                                  | *boolean*                                                    | :heavy_minus_sign:                                           | N/A                                                          |                                                              |