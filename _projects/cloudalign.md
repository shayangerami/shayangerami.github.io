---
layout: page
title: CloudAlign
description: Global-to-local 3D point-cloud registration with Open3D
img: # optional card image, e.g. assets/img/projects/cloudalign.jpg
importance: 2
category: independent
---

**CloudAlign: 3D Point-Cloud Registration**

ICP alone converges well only when two point clouds start close together. CloudAlign adds a global alignment step first so registration also succeeds from poor initial poses.

#### Highlights

- Built an Open3D pipeline combining FPFH descriptors, RANSAC global alignment, and ICP refinement.
- Improved pose-recovery success over ICP alone from 69% to 99% across 100 test pairs, and from 15% to 97% under large rotations.
- Median CPU runtime of 0.151 s per pair.
