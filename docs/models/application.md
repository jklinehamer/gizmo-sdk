# Application

The Application object

## Example Usage

```typescript
import { Application } from "@gizmo-os/sdk/models";

let value: Application = {
  id: "<id>",
  orgId: "<id>",
  createdAt: 3684.3,
  status: "FUNDED",
  primaryBorrowerFirstName: "<value>",
  primaryBorrowerLastName: "<value>",
  primaryBorrowerEmail: "<value>",
  primaryBorrowerPhone: "<value>",
  subjectPropertyState: "nc",
  leadProviderSlug: "<value>",
};
```

## Fields

| Field                                          | Type                                           | Required                                       | Description                                    |
| ---------------------------------------------- | ---------------------------------------------- | ---------------------------------------------- | ---------------------------------------------- |
| `id`                                           | *string*                                       | :heavy_check_mark:                             | N/A                                            |
| `orgId`                                        | *string*                                       | :heavy_check_mark:                             | N/A                                            |
| `createdAt`                                    | *number*                                       | :heavy_check_mark:                             | N/A                                            |
| `updatedAt`                                    | *number*                                       | :heavy_minus_sign:                             | N/A                                            |
| `status`                                       | [models.Milestone](../models/milestone.md)     | :heavy_check_mark:                             | N/A                                            |
| `primaryBorrowerFirstName`                     | *string*                                       | :heavy_check_mark:                             | N/A                                            |
| `primaryBorrowerLastName`                      | *string*                                       | :heavy_check_mark:                             | N/A                                            |
| `primaryBorrowerEmail`                         | *string*                                       | :heavy_check_mark:                             | N/A                                            |
| `primaryBorrowerPhone`                         | *string*                                       | :heavy_check_mark:                             | N/A                                            |
| `primaryBorrowerDateOfBirth`                   | *string*                                       | :heavy_minus_sign:                             | N/A                                            |
| `primaryBorrowerSsn`                           | *string*                                       | :heavy_minus_sign:                             | N/A                                            |
| `subjectPropertyState`                         | [models.State](../models/state.md)             | :heavy_check_mark:                             | The two-letter state abbreviation in lowercase |
| `subjectPropertyStreetAddress`                 | *string*                                       | :heavy_minus_sign:                             | N/A                                            |
| `subjectPropertyCity`                          | *string*                                       | :heavy_minus_sign:                             | N/A                                            |
| `subjectPropertyZip`                           | *string*                                       | :heavy_minus_sign:                             | N/A                                            |
| `loanPurpose`                                  | [models.LoanPurpose](../models/loanpurpose.md) | :heavy_minus_sign:                             | N/A                                            |
| `losId`                                        | *string*                                       | :heavy_minus_sign:                             | N/A                                            |
| `crmId`                                        | *string*                                       | :heavy_minus_sign:                             | N/A                                            |
| `leadProviderSlug`                             | *string*                                       | :heavy_check_mark:                             | N/A                                            |