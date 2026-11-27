---
name: particle-morph-landing
description: >
  Particle morph landing pages — logo to map to camera to gate, GPU morph, bloom and vignette. Use for cinematic scroll landings.
license: MIT
metadata:
  author: Anya, on behalf of olieolay
  version: "1.0.0"
  updated: "2026-11-24"
---

# Particle Morph Landing

You build cinematic particle landing pages: a logo morphs into a map, a number, a camera, then a gate.

## Rules
- ONE THREE.Points + ShaderMaterial, GPU morph between target point sets. 12,000 particles desktop, 6,000 mobile. Morph window 55% per particle, stagger 0.45.
- Beats (durations): logo 2.5 s, map 1.8 s, number 1.5 s, camera 1.5 s, gate 2.0 s. Hold 0.8 s + breathe 0.4 s between beats. Total about 15.8 s.
- Easing: power3.inOut for logo and gate, power2.inOut for the rest.
- Effects: Bloom strength 0.5, radius 0.5, threshold 0.8; ACES tone mapping, exposure about 1.1; vignette last.
- Logo: use the official logo exactly as supplied, never redrawn. If particle sampling is not faithful, show the real logo as an image with particles orbiting it.
- Respect prefers-reduced-motion: skip morph, show the final shape statically.
- Never use random rainbow particles or generic AI-template gradients.

## Workflow
1. List the 5 shapes in order and their durations.
2. Sample each shape to the same particle count.
3. Build the shader morph, then bloom/vignette, then the call-to-action after the camera stops.
4. Test headless and on a real device; measure FPS before calling it done.

## Identity
Tagline exact: Explore Indonesia Through Instanusantara. Founded 1 March 2012. Navy + gold, batik, Candi Bentar.

