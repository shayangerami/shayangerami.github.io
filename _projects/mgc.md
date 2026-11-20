---
layout: page
title: MGC
description: Missed-Guidance Correction for conditions that change mid-generation in diffusion and flow models
img: # optional card image, e.g. assets/img/projects/mgc.jpg
importance: 2
category: research
---

**What a Late Condition Misses: Correcting Mid-Trajectory Condition Changes** _(manuscript under review)_

When a new condition arrives partway through sampling, simply switching to it leaves the sample missing the guidance it would have received earlier. Missed-Guidance Correction (MGC) is a training-free method that adapts diffusion and flow samplers to conditions that arrive mid-generation.

#### Method

- Estimates the missed guidance from two to five probes of earlier sampler states.
- Applies a single correction at the switch.
- Shows that historical guidance carries target-specific information beyond the condition difference at the switch, and that semantic correction can succeed without recovering the restart state.

#### Results

- **Image generation.** Using two probes, concept insertion success rose from 19.6% to 49.7% on Stable Diffusion 2.1 and from 41.4% to 71.0% on SD3.5, averaged across switch times on prompt pairs where restarting succeeds.
- **Compute.** MGC needs 8% more model evaluations than direct switching and outperforms equal-compute rewinding by 26.1 percentage points on SD2.1.
- **Audio-visual speech enhancement.** With delayed lip-video conditioning, MGC recovers 86.1% of the full audio-visual SI-SDR gain versus 49.4% for direct switching on the held-out speaker, and 72.9% versus 28.7% on unseen speakers and noise types.
