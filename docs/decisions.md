# Product decision log

## Decision: use measured gauge, not hook size, as the geometry input

**Context**
Hook size does not uniquely determine stitch dimensions. Yarn, tension and stitch behaviour also matter.

**Decision**
Use the measured stitch and row gauge from the user's actual swatch to calculate physical pattern proportions.

**Product effect**
Image conversion becomes a physical-geometry problem rather than simple pixel resizing.

---

## Decision: model a garment as multiple independent panels

**Context**
A single chart could not represent a complete shirt or sweater workflow. Front, back and sleeves may carry different designs and production state.

**Decision**
Make a project own multiple panels, each with independent design/grid/palette state while remaining part of one garment project.

**Product effect**
Panel switching, duplicate/move actions, aggregate production and garment-aware exports become possible.

---

## Decision: keep manual correction as a core workflow

**Context**
Automatic image conversion and background removal can damage important detail or produce impractical stitch regions.

**Decision**
Treat generation as a starting point. Preserve editing, undo, regeneration and explicit protection controls.

**Product effect**
The system supports human judgement instead of depending on perfect automation.

---

## Decision: replace weak 3D mock-up direction with flat approval views

**Context**
The 3D direction added substantial technical complexity without producing a sufficiently trustworthy client preview.

**Decision**
Use flat panel previews for front, back, left sleeve and right sleeve. Front/back views no longer include attached sleeves because sleeves are represented separately.

**Product effect**
The preview more directly matches the client's approval job and is easier to validate.

---

## Decision: keep SaaS downstream of workflow validation

**Context**
Accounts, sync and subscriptions can make a product look commercial without proving that the production workflow is valuable.

**Decision**
Prioritise local workflow correctness and external maker validation before SaaS infrastructure.

**Product effect**
The roadmap remains focused on product evidence instead of platform complexity.
