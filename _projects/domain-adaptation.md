---
layout: page
title: CT-to-X-Ray Domain Adaptation
description: Deep domain adaptation from chest CT to chest X-ray classification
img: # optional card image, e.g. assets/img/projects/domain-adaptation.jpg
importance: 3
category: independent
github: https://github.com/shayangerami/DomainAdaptation
---

**Deep Domain Adaptation for CT-to-X-Ray Classification**

A classifier trained on chest CT scans transfers poorly to chest X-rays. This project compares ways of adapting it to the X-ray domain.

#### Highlights

- Compared fine-tuning, DANN, CORAL, and MMD using a RadImageNet-pretrained ResNet-50.
- The best configuration raised target X-ray test accuracy from 60.87% to 97.83% in the project evaluation.

Code: [github.com/shayangerami/DomainAdaptation](https://github.com/shayangerami/DomainAdaptation)
