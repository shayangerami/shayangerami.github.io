---
layout: page
title: SENTRY
description: Spike-based event filtering that triggers selective deep inference at the edge (ACM GLSVLSI 2026)
img: # optional card image, e.g. assets/img/projects/sentry.jpg
importance: 7
category: research
related_publications: true
---

**SENTRY: Spiking Event Reasoning for Selective Deep Inference in Event-Driven Edge Vision** {% cite gerami2026sentry %}

Event cameras produce spikes whenever brightness changes, but not every burst of activity is worth running a deep model on or transmitting. SENTRY filters event-camera spikes by region to decide when to trigger deep inference.

#### Highlights

- Developed hierarchical event filtering that combines regional spike-rate gating with spatial confirmation to trigger selective vision inference.
- On an evaluated surveillance sequence, improved transmission precision from 41% to 67% and reduced false-positive transmissions from 65 to 28 compared with a global spike-rate baseline.
