# UpdateApplicationRequest

## Example Usage

```typescript
import { UpdateApplicationRequest } from "@gizmo-os/sdk/models/operations";

let value: UpdateApplicationRequest = {
  id: "423",
  applicationPatch: {
    id: {
      id: "423",
    },
    status: "CONDITIONALLY_APPROVED",
  },
};
```

## Fields

| Field                                                       | Type                                                        | Required                                                    | Description                                                 | Example                                                     |
| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |
| `id`                                                        | *string*                                                    | :heavy_check_mark:                                          | N/A                                                         | 423                                                         |
| `applicationPatch`                                          | [models.ApplicationPatch](../../models/applicationpatch.md) | :heavy_check_mark:                                          | N/A                                                         |                                                             |