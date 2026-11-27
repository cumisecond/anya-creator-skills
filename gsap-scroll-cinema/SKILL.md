---
name: gsap-scroll-cinema
description: >
  GSAP scroll cinema — ScrollTrigger, MotionPath, SplitText, timelines for camera journeys and kinetic type. Use for scroll-driven stories and letter animation.
license: MIT
metadata:
  author: Anya, on behalf of olieolay
  version: "1.0.0"
  updated: "2026-11-24"
---

# GSAP Scroll Cinema

You direct scroll-driven cinema with GSAP: camera journeys, kinetic type, and timelines.

## Rules
- Vanilla GSAP, local bundle. ScrollTrigger scrub is the main mode for corridors; MotionPath for letters and camera paths; SplitText for kinetic type.
- Snake letters (chosen variant): letters follow a wavy elliptical MotionPath, 26 s per loop, one after another. Text exact: Explore Indonesia Through Instanusantara. INSTANUSANTARA red (#e5484d), the rest white.
- MorphSVG is only for 2D SVG, never for 3D particles.
- Timelines: name every beat, set durations and easings first, then code. One hero moves at a time.
- Always set fromCurrent correctly on MotionPath, or letters will wander to the header.
- Respect prefers-reduced-motion: letters become a static ring, scroll becomes button jumps.

## Workflow
1. Map the scroll journey to beats and camera stops.
2. Build the GSAP timeline with labels.
3. Add kinetic type last, test one full loop.
4. Verify on desktop and phone, 0 console errors.

## Identity
Tagline exact: Explore Indonesia Through Instanusantara. Founded 1 March 2012. Never show partner/sponsor logos.

