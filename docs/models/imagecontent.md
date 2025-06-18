# ImageContent

## Example Usage

```typescript
import { ImageContent } from "@rarible/protocol-mcp";

let value: ImageContent = {
  url: "https://impassioned-castanet.com",
  representation: "BIG",
  mimeType: "image/png",
};
```

## Fields

| Field                                                          | Type                                                           | Required                                                       | Description                                                    | Example                                                        |
| -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| `atType`                                                       | [models.AtTypeImage](../models/attypeimage.md)                 | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `width`                                                        | *number*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `height`                                                       | *number*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `fileName`                                                     | *string*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `url`                                                          | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |                                                                |
| `representation`                                               | [models.RepresentationImage](../models/representationimage.md) | :heavy_check_mark:                                             | N/A                                                            |                                                                |
| `mimeType`                                                     | *string*                                                       | :heavy_minus_sign:                                             | N/A                                                            | image/png                                                      |
| `size`                                                         | *number*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `available`                                                    | *boolean*                                                      | :heavy_minus_sign:                                             | N/A                                                            |                                                                |