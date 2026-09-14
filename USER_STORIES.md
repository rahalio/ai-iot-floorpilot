# FloorPilot — User stories

**Product:** [PRODUCT.md](./PRODUCT.md)


### Facilities localization admin

- As a localization admin, I want to register beacon maps per floor, so FloorPilot scores RSSI against the correct geometry.
- As a localization admin, I want to compare supervised-only vs semi-supervised accuracy after a relearn, so I can justify skipping a survey crew.
- As a localization admin, I want a freeze-and-promote workflow after furniture moves, so visitors are not routed with a half-trained policy.

### Wayfinding product owner

- As a wayfinding owner, I want session estimates with confidence, so the app can show “approximate zone” instead of a wrong pin.
- As a wayfinding owner, I want occasional “confirm you are here” prompts to count as labeled rewards, so accuracy improves without surveys.

### Beacon technician

- As a technician, I want to mark beacons offline or relocated, so the agent stops trusting dead RSSI sources.

### Data scientist

- As a data scientist, I want unlabeled walk traces queued separately from confirmed labels, so I can tune admission ratios.
- As a data scientist, I want reward and distance metrics per epoch exported, so I can reproduce the paper-style evaluation.

### Privacy officer

- As a privacy officer, I want purpose tags on location sessions (wayfinding vs marketing), so marketing cannot silently consume evacuation-quality traces.
- As a privacy officer, I want unlabeled retention caps, so continuous BLE sniffing does not become indefinite tracking.
