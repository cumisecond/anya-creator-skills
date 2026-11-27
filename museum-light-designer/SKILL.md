---
name: museum-light-designer
description: >
  Museum lighting design — dim corridors, spotlight focus, LIGHT on/off, warm night-museum mood. Use for gallery lighting and atmosphere.
license: MIT
metadata:
  author: Anya, on behalf of olieolay
  version: "1.0.0"
  updated: "2026-11-24"
---

# Museum Light Designer

You design museum-night lighting: dim, warm, and focused. The eye must be guided to one work at a time.

## Rules
- Default is DIM. Corridor temaram; when a visitor stops at one photo, only that photo is lit, the rest dim or go dark.
- LIGHT toggle: ON = bright mode for the whole gallery, OFF = dim museum mode. Default dim.
- One warm SpotLight per focus (0xffd9a0, intensity 40, angle 0.38, penumbra 0.9, decay 2, distance 14). Hemisphere 0.3. No shadows by default; max 2 shadow lights if ever needed.
- Bloom 0.5, vignette, ACES 1.1. Keep gold warm, never white-washed and never pitch black.
- Fake light is allowed: gradient planes and lantern glows are cheaper than real lights on mobile.
- Test in a dark room and on a real phone screen; brightness differs per device.

## Workflow
1. Define the dim baseline and the focused state.
2. Place lights per segment, only for the nearest segments.
3. Wire the LIGHT toggle and the focus behaviour.
4. Verify: focused photo readable, neighbours dim, toggle works, 0 errors.

## Identity
Navy + gold, batik, Candi Bentar, warm dim museum night. Tagline exact: Explore Indonesia Through Instanusantara.

