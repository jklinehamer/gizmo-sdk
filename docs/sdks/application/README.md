# Application
(*application*)

## Overview

### Available Operations

* [getApplication](#getapplication) - Get Application
* [updateApplication](#updateapplication) - Update Application
* [createApplication](#createapplication) - Create Application

## getApplication

Get Application

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getApplication" method="get" path="/applications/{id}" -->
```typescript
import { Gizmo } from "@gizmo-os/sdk";

const gizmo = new Gizmo({
  bearerAuth: process.env["GIZMO_BEARER_AUTH"] ?? "",
});

async function run() {
  const result = await gizmo.application.getApplication("<id>");

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { GizmoCore } from "@gizmo-os/sdk/core.js";
import { applicationGetApplication } from "@gizmo-os/sdk/funcs/applicationGetApplication.js";

// Use `GizmoCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const gizmo = new GizmoCore({
  bearerAuth: process.env["GIZMO_BEARER_AUTH"] ?? "",
});

async function run() {
  const res = await applicationGetApplication(gizmo, "<id>");
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("applicationGetApplication failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                           | *string*                                                                                                                                                                       | :heavy_check_mark:                                                                                                                                                             | N/A                                                                                                                                                                            |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Application](../../models/application.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.ErrorResponse     | 400                      | application/json         |
| errors.GizmoDefaultError | 4XX, 5XX                 | \*/\*                    |

## updateApplication

Update Application

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateApplication" method="patch" path="/applications/{id}" -->
```typescript
import { Gizmo } from "@gizmo-os/sdk";

const gizmo = new Gizmo({
  bearerAuth: process.env["GIZMO_BEARER_AUTH"] ?? "",
});

async function run() {
  const result = await gizmo.application.updateApplication("<id>");

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { GizmoCore } from "@gizmo-os/sdk/core.js";
import { applicationUpdateApplication } from "@gizmo-os/sdk/funcs/applicationUpdateApplication.js";

// Use `GizmoCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const gizmo = new GizmoCore({
  bearerAuth: process.env["GIZMO_BEARER_AUTH"] ?? "",
});

async function run() {
  const res = await applicationUpdateApplication(gizmo, "<id>");
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("applicationUpdateApplication failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                           | *string*                                                                                                                                                                       | :heavy_check_mark:                                                                                                                                                             | N/A                                                                                                                                                                            |
| `requestBody`                                                                                                                                                                  | [operations.UpdateApplicationRequestBody](../../models/operations/updateapplicationrequestbody.md)                                                                             | :heavy_minus_sign:                                                                                                                                                             | N/A                                                                                                                                                                            |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[any](../../models/.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.ErrorResponse     | 400                      | application/json         |
| errors.GizmoDefaultError | 4XX, 5XX                 | \*/\*                    |

## createApplication

Create Application

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createApplication" method="post" path="/applications" -->
```typescript
import { Gizmo } from "@gizmo-os/sdk";

const gizmo = new Gizmo({
  bearerAuth: process.env["GIZMO_BEARER_AUTH"] ?? "",
});

async function run() {
  const result = await gizmo.application.createApplication();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { GizmoCore } from "@gizmo-os/sdk/core.js";
import { applicationCreateApplication } from "@gizmo-os/sdk/funcs/applicationCreateApplication.js";

// Use `GizmoCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const gizmo = new GizmoCore({
  bearerAuth: process.env["GIZMO_BEARER_AUTH"] ?? "",
});

async function run() {
  const res = await applicationCreateApplication(gizmo);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("applicationCreateApplication failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateApplicationRequest](../../models/operations/createapplicationrequest.md)                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateApplicationResponse](../../models/operations/createapplicationresponse.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.ErrorResponse     | 400                      | application/json         |
| errors.GizmoDefaultError | 4XX, 5XX                 | \*/\*                    |