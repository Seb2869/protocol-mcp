# SignatureValidationForm

## Example Usage

```typescript
import { SignatureValidationForm } from "@rarible/protocol-mcp";

let value: SignatureValidationForm = {
  signer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  message: "<value>",
  signature: "<value>",
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     | Example                                                                         |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `signer`                                                                        | *string*                                                                        | :heavy_check_mark:                                                              | Blockchain address in Union format `${blockchainGroup}:${token}`                | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                             |
| `publicKey`                                                                     | *string*                                                                        | :heavy_minus_sign:                                                              | The creator's public key                                                        |                                                                                 |
| `message`                                                                       | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |                                                                                 |
| `signature`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | Digital signature of the signer                                                 |                                                                                 |
| `algorithm`                                                                     | *string*                                                                        | :heavy_minus_sign:                                                              | Algorithm used for signature generation (don't specify if default algo is used) |                                                                                 |
| `weight`                                                                        | *number*                                                                        | :heavy_minus_sign:                                                              | Weight arg (only for Flow)                                                      |                                                                                 |