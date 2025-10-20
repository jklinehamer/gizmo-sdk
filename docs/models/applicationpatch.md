# ApplicationPatch

## Example Usage

```typescript
import { ApplicationPatch } from "@gizmo-os/sdk/models";

let value: ApplicationPatch = {
  id: {
    id: "423",
  },
  status: "RESUBMITTAL",
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `id`                                                                 | [models.Id](../models/id.md)                                         | :heavy_check_mark:                                                   | N/A                                                                  |
| `status`                                                             | [models.ApplicationPatchStatus](../models/applicationpatchstatus.md) | :heavy_check_mark:                                                   | N/A                                                                  |