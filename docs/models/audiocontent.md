# AudioContent

## Example Usage

```typescript
import { AudioContent } from "@rarible/protocol-mcp";

let value: AudioContent = {
  url: "https://substantial-moment.name/",
  representation: "PORTRAIT",
  mimeType: "image/png",
};
```

## Fields

| Field                                                          | Type                                                           | Required                                                       | Description                                                    | Example                                                        |
| -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| `atType`                                                       | [models.AtTypeAudio](../models/attypeaudio.md)                 | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `fileName`                                                     | *string*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `url`                                                          | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |                                                                |
| `representation`                                               | [models.RepresentationAudio](../models/representationaudio.md) | :heavy_check_mark:                                             | N/A                                                            |                                                                |
| `mimeType`                                                     | *string*                                                       | :heavy_minus_sign:                                             | N/A                                                            | image/png                                                      |
| `size`                                                         | *number*                                                       | :heavy_minus_sign:                                             | N/A                                                            |                                                                |
| `available`                                                    | *boolean*                                                      | :heavy_minus_sign:                                             | N/A                                                            |                                                                |