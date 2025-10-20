<!-- Start SDK Example Usage [usage] -->
```typescript
import { Gizmo } from "@gizmo-os/sdk";

const gizmo = new Gizmo();

async function run() {
  const result = await gizmo.applications.get({
    id: "423",
  });

  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->