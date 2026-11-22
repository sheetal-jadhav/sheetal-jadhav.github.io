---
title: "Replicating a Biophysical Model of HVC"
project: true
weight: 4
status: "Current"
summary: "An independent replication, for ReScience C, of a biophysical three-class network model of the songbird premotor nucleus HVC (Bou Diab, Chammas & Daou, eLife 2025), rebuilt from the published text alone."
tags: ["Birdsong", "HVC", "Replication", "Modelling"]
cover:
  image: "/images/projects/hvc-replication.png"
  alt: "Spike raster of 120 HVC(RA) neurons firing in order, one after another, across about 250 ms"
  caption: "Sequence propagation in the replicated model: all 120 HVC(RA) neurons burst in chain order."
  hiddenInSingle: false
hideMeta: true
---

**Code:** [github.com/sheetal-jadhav/rescience-zeina-boudiab-2025-hvc](https://github.com/sheetal-jadhav/rescience-zeina-boudiab-2025-hvc)

## About

HVC is the premotor nucleus that drives the precise timing of zebra finch song. Bou Diab, Chammas & Daou (2025, *eLife* 14:RP105526) proposed a conductance-based network of its three neuron classes (HVC(RA) projection neurons, HVC(X) projection neurons and interneurons) to explain how a stereotyped sequence of activity propagates through it.

I re-implemented the model from the published description only, without opening the authors' code until my own figures existed, for submission to [ReScience C](https://rescience.github.io/). The model is written as a reusable Python library (SciPy RK45 integration, with fixed-step RK4 as a check), and a second, independent implementation in Brian2 confirms the results.

## Findings

- **Reproduced:** the HVC(RA) chain. In 50 of 50 random networks, activity propagates through all 120 HVC(RA) neurons in order.
- **Not reproduced from the published description:** the HVC(X) rebound bursts, the dense interneuron firing, the calibration of cell pairs, and the fragility results of the perturbation experiments.
- Every gap, typo and modelling choice is documented in the repository's issues log.
