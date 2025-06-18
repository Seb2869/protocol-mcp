# VideoContent

## Example Usage

```typescript
import { VideoContent } from "@rarible/protocol-mcp";

let value: VideoContent = {
  url: "https://velvety-offset.name",
  representation: "INITIAL",
  mimeType: "image/png",
};
```

## Fields

| Field                                                          | Type                                                           | Required                                                       | Description                                                    | Example                                                        |
| -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| `atType`                                                       | [models.AtTypeVideo](../models/attypevideo.md)                 | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `width`                                                        | *number*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `height`                                                       | *number*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `fileName`                                                     | *string*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `url`                                                          | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |                                                                |
| `representation`                                               | [models.RepresentationVideo](../models/representationvideo.md) | :heavy_check_mark:                                             | N/A                                                            |                                                                |
| `mimeType`                                                     | *string*                                                       | :heavy_minus_sign:                                             | N/A                                                            | image/png                                                      |
| `size`                                                         | *number*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `available`                                                    | *boolean*                                                      | :heavy_minus_sign:                                             | N/A                                                            |                                                                |