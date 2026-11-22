---
title: "Brain Networks for Face Processing"
project: true
weight: 4
summary: "Seed-based functional connectivity analysis of the open-source Haxby fMRI dataset, mapping the wider brain network involved in face processing. Homi Bhabha Centre for Science Education, Mumbai."
tags: ["fMRI", "Functional connectivity", "Face processing", "Cognitive science"]
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
