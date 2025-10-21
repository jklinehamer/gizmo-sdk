<!-- Start SDK Example Usage [usage] -->
```typescript
import { Gizmo } from "@gizmo-os/sdk";

const gizmo = new Gizmo({
  bearerAuth: process.env["GIZMO_BEARER_AUTH"] ?? "",
});

async function run() {
  const result = await gizmo.applications.get("<id>");

  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->