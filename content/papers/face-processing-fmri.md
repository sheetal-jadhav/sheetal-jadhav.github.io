---
title: "Role of Limbic System in Face Recognition Circuits"
project: true
weight: 7
summary: "Seed-based functional connectivity analysis of the open-source Haxby fMRI dataset, mapping the wider brain network involved in face processing. Homi Bhabha Centre for Science Education, Mumbai."
tags: ["fMRI", "Functional connectivity", "Face processing", "Cognitive science"]
credit: "Cover image: De Negri, Simone, Caruana & Gerbella (2026), Brain Structure and Function 231:72, Fig. 5A,B (CC BY 4.0)"
cover:
  image: "/images/projects/face-processing-fmri.jpg"
  alt: "Tractography in a template human brain: white-matter fibres, including the cingulum bundle, linking anterior cingulate and ventromedial prefrontal regions shown as coloured spheres"
  caption: "Cover image: white-matter connections between cingulate and prefrontal nodes of the frontal face network, from Fig. 5A,B of De Negri B, Simone L, Caruana F, Gerbella M (2026). [Inside the frontal face network: multimodal evidence for distinct emotional and motor resonance circuits](https://doi.org/10.1007/s00429-026-03125-5). *Brain Structure and Function* 231:72. © The Author(s) 2026, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)."
  hiddenInSingle: false
hideMeta: true
---

Visiting Research Fellow, Homi Bhabha Centre for Science Education (HBCSE), Mumbai · January 2020 – July 2021<br>
Supervisor: Prof. Sanjay Chandrasekharan

**Poster:** Sheetal Jadhav and Sanjay Chandrasekharan, *"She saw me and made a face: functional network analysis reveals role of the limbic system in face recognition"*. 7th Annual Conference of Cognitive Science (ACCS7), Indian Institute of Science, Bangalore (online), 23 January 2021. [Abstract book](https://drive.google.com/file/d/13f0but6u5SQe_gL0B4xqjR85k3Ot84Kf/view), pp. 44–45.

## About

Faces carry some of the most important social information we receive: identity, emotional state and where someone is looking. Face processing is therefore tied to emotion, action and social cognition, which suggests that it recruits brain regions well beyond the core face-selective areas. This project asked which wider regions take part in face processing, and what they might contribute.

## Methods

- **Data:** the Haxby fMRI dataset, an open dataset from a study of face and object representation in the human brain. Six subjects each passively viewed greyscale images of eight object categories, including faces, in 12 runs.
- **Preprocessing:** brain extraction and motion correction in FSL.
- **Seed-based functional connectivity:** with Nilearn in Python, the BOLD signal of a seed region, the occipital fusiform gyrus (part of the core face-processing network), was correlated with every other voxel in the brain to build a functional connectivity map, followed by a group analysis across all six subjects.

## Findings

- The face-correlated network was bilateral and included the superior and middle frontal gyri, the cingulate gyrus, the insula and the medial occipitotemporal gyrus.
- The cingulate gyrus points to a role for the limbic system: making sense of, and acting on, facial expressions and emotions, which a purely geometric recognition of a face does not provide.
- The posterior cingulate is part of the default mode network, which suggests that internally directed processes such as memory retrieval and planning are also part of face recognition.
