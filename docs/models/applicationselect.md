# ApplicationSelect

## Example Usage

```typescript
import { ApplicationSelect } from "@gizmo-os/sdk/models";

let value: ApplicationSelect = {
  id: "<id>",
  createdAt: 4441.54,
  status: "CONTACTED",
  timezone: "Africa/Khartoum",
  primaryBorrowerId: "<id>",
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `id`                                                                   | *string*                                                               | :heavy_check_mark:                                                     | N/A                                                                    |
| `createdAt`                                                            | *number*                                                               | :heavy_check_mark:                                                     | N/A                                                                    |
| `updatedAt`                                                            | *number*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `losId`                                                                | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `crmId`                                                                | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `losApplicationId`                                                     | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `assignedUserId`                                                       | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `subjectPropertyId`                                                    | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `status`                                                               | [models.ApplicationSelectStatus](../models/applicationselectstatus.md) | :heavy_check_mark:                                                     | N/A                                                                    |
| `nextAppointmentAt`                                                    | *number*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `timezone`                                                             | *string*                                                               | :heavy_check_mark:                                                     | Example: "America/New_York                                             |
| `timezoneOffset`                                                       | *number*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `primaryBorrowerId`                                                    | *string*                                                               | :heavy_check_mark:                                                     | N/A                                                                    |