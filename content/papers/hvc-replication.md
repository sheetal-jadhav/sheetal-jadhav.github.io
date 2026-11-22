---
title: "Replicating a Biophysical Model of HVC"
project: true
weight: 2
status: "Current"
summary: "An independent replication of a biophysical three-class network model of the songbird premotor nucleus HVC (Bou Diab, Chammas & Daou, eLife 2025), rebuilt from the published text alone."
tags: ["Birdsong", "HVC", "Replication", "Modelling"]
cover:
  image: "/images/projects/hvc-replication-fig5.png"
  alt: "Voltage traces of a presynaptic HVC(RA) neuron bursting and a postsynaptic HVC(RA) neuron responding a few milliseconds later, for two values of AMPA conductance (A) and A-type potassium conductance (B)"
  caption: "Replicated Fig 5: the synaptic delay between consecutive HVC(RA) neurons, and how it changes with AMPA conductance (A) and A-type potassium conductance (B)."
  hiddenInSingle: false
hideMeta: true
---

**Code:** [github.com/sheetal-jadhav/rescience-zeina-boudiab-2025-hvc](https://github.com/sheetal-jadhav/rescience-zeina-boudiab-2025-hvc)

## About

HVC is the premotor nucleus that drives the precise timing of zebra finch song. Bou Diab, Chammas & Daou (2025, *eLife* 14:RP105526) proposed a conductance-based network of its three neuron classes (HVC(RA) projection neurons, HVC(X) projection neurons and interneurons) to explain how a stereotyped sequence of activity propagates through it. This project is an independent replication of that model.

## Methods

- **Hodgkin–Huxley-type neurons.** Each cell class is a conductance-based model with its own set of ionic currents, connected by AMPA and GABA synapses according to the paper's wiring rules.
- **Reusable Python library.** The model is written as a small library, with the network wiring given as declarative specifications. Simulations use SciPy's adaptive RK45 solver (the same method as MATLAB's ode45), checked against a fixed-step RK4 integrator.
- **A second, independent implementation.** The model was also rebuilt in Brian2, and both versions give the same results.
- **Many random networks, not one.** Each result is tested across many randomly wired networks (for example 50 networks for sequence propagation), together with robustness and numerical checks.

## Findings

- **Reproduced:** the HVC(RA) chain. In 50 of 50 random networks, activity propagates through all 120 HVC(RA) neurons in order.
- **Not reproduced from the published description:** the HVC(X) rebound bursts, the dense interneuron firing, the calibration of cell pairs, and the fragility results of the perturbation experiments.
- Every gap, typo and modelling choice is documented in the repository's issues log.
