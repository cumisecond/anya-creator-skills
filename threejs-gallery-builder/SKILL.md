---
name: threejs-gallery-builder
description: >
  Build vanilla Three.js galleries, rotundas, and corridors — local bundle, no CDN, no React. Use for 3D exhibition rooms, 360 galleries, and first-person corridors.
license: MIT
metadata:
  author: Anya, on behalf of olieolay
  version: "1.0.0"
  updated: "2026-11-24"
---

# Three.js Gallery Builder

You build 3D galleries in vanilla Three.js, single file, local bundle (./three.module.js). No CDN, no React, no Google Fonts (Georgia serif + system-ui).

## Rules
- One renderer, one scene per mode. Dispose renderers and textures when leaving a scene.
- Rotunda: cylindrical wall, warm light, reflective floor, drag/swipe/keyboard navigation.
- Corridor: first-person, 0.9 s per segment, sine.inOut, head-bob 0.04. Stop BEFORE the gate (about 4.5 units away), then show the call-to-action.
- Lighting: one warm SpotLight (0xffd9a0, intensity 40, angle 0.38, penumbra 0.9, decay 2, distance 14, no shadow) + dim Hemisphere (0.3). Only the focused work is lit.
- Performance: pixelRatio max 2, throttle hover raycasts to about 150 ms, clamp anisotropy to 4. If FPS is below 45, lower particles first, then bloom.
- Test 1920x1080, 1366x768, and a real phone. If the phone contradicts a local test, the phone wins.
- Never auto-enter the gallery. Entry only by click. Never show partner/sponsor logos.

## Workflow
1. Define rooms, order, and zones before writing code.
2. Build the rotunda, then the corridor, then the plaza.
3. Add lighting and focus behaviour last.
4. Verify live: every room reachable, every button works, 0 console errors, no overflow.

## Identity
Tagline exact: Explore Indonesia Through Instanusantara. Founded 1 March 2012. Identity: navy + gold, batik, Candi Bentar, warm dim museum night.

