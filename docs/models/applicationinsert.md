# ApplicationInsert

## Example Usage

```typescript
import { ApplicationInsert } from "@gizmo-os/sdk/models";

let value: ApplicationInsert = {
  firstName: "Mohammad",
  lastName: "Abshire",
  phone: "(335) 291-5980 x56558",
  state: "ct",
  leadProviderSlug: "<value>",
  orgId: "<id>",
};
```

## Fields

| Field                              | Type                               | Required                           | Description                        |
| ---------------------------------- | ---------------------------------- | ---------------------------------- | ---------------------------------- |
| `crmId`                            | *string*                           | :heavy_minus_sign:                 | N/A                                |
| `firstName`                        | *string*                           | :heavy_check_mark:                 | N/A                                |
| `lastName`                         | *string*                           | :heavy_check_mark:                 | N/A                                |
| `email`                            | *string*                           | :heavy_minus_sign:                 | N/A                                |
| `phone`                            | *string*                           | :heavy_check_mark:                 | N/A                                |
| `streetAddress`                    | *string*                           | :heavy_minus_sign:                 | N/A                                |
| `city`                             | *string*                           | :heavy_minus_sign:                 | N/A                                |
| `state`                            | [models.State](../models/state.md) | :heavy_check_mark:                 | N/A                                |
| `zip`                              | *string*                           | :heavy_minus_sign:                 | N/A                                |
| `leadProviderSlug`                 | *string*                           | :heavy_check_mark:                 | N/A                                |
| `orgId`                            | *string*                           | :heavy_check_mark:                 | N/A                                |