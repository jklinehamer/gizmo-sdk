# CreateApplicationRequest

## Example Usage

```typescript
import { CreateApplicationRequest } from "@gizmo-os/sdk/models/operations";

let value: CreateApplicationRequest = {
  primaryBorrowerFirstName: "<value>",
  primaryBorrowerLastName: "<value>",
  primaryBorrowerEmail: "<value>",
  primaryBorrowerPhone: "<value>",
  subjectPropertyState: "sc",
  leadProviderSlug: "<value>",
};
```

## Fields

| Field                                             | Type                                              | Required                                          | Description                                       |
| ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- |
| `primaryBorrowerFirstName`                        | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `primaryBorrowerLastName`                         | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `primaryBorrowerEmail`                            | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `primaryBorrowerPhone`                            | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `primaryBorrowerDateOfBirth`                      | *string*                                          | :heavy_minus_sign:                                | N/A                                               |
| `primaryBorrowerSsn`                              | *string*                                          | :heavy_minus_sign:                                | N/A                                               |
| `subjectPropertyState`                            | [models.State](../../models/state.md)             | :heavy_check_mark:                                | The two-letter state abbreviation in lowercase    |
| `subjectPropertyStreetAddress`                    | *string*                                          | :heavy_minus_sign:                                | N/A                                               |
| `subjectPropertyCity`                             | *string*                                          | :heavy_minus_sign:                                | N/A                                               |
| `subjectPropertyZip`                              | *string*                                          | :heavy_minus_sign:                                | N/A                                               |
| `loanPurpose`                                     | [models.LoanPurpose](../../models/loanpurpose.md) | :heavy_minus_sign:                                | N/A                                               |
| `losId`                                           | *string*                                          | :heavy_minus_sign:                                | N/A                                               |
| `crmId`                                           | *string*                                          | :heavy_minus_sign:                                | N/A                                               |
| `leadProviderSlug`                                | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `teamId`                                          | *string*                                          | :heavy_minus_sign:                                | N/A                                               |