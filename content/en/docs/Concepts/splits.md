---
title: "Split Expression"
linkTitle: "Split Expression"
categories: ["overview","help"]
tags: ["Split","Expression_pattern","transgene","FlyLight"]
weight: 30
description: >
  This techniques work by driving the expression of target transgenes at the intersection between the expression patterns of two hemi-driver transgenes.
---

Thousands of hemi-driver transgenes are now available, meaning that millions of combinations/[splits](/tags/split/) are possible, each targeting some precise subset of the 10s-100s of thousands of neurons in a fly Central Nervous System (CNS).  Finding the right combination for an experiment is a serious bottleneck for researchers.

[FlyBase](https://flybase.org/) & [Virtual Fly Brain (VFB)](https://virtualflybrain.org) solve this problem by curating information and images recording where expression is driven by combinations of hemi-drivers.  Each combination gets a standard name on VFB reflecting the names of the component hemidrivers (see figure below) and is also associated with any short names for the combination used in the literature (e.g. "[P{VT017411-GAL4.DBD} ∩ P{VT019018-p65.AD} expression pattern](https://v2.virtualflybrain.org/org.geppetto.frontend/geppetto?id=VFBexp_FBtp0123314FBtp0119891)" has_exact_synonym: SS02256")

<img src="/images/splits_images.png" max-width="50%" alt="This techniques work by driving the expression of target transgenes at the intersection between the expression patterns of two hemi-driver transgenes." ><img src="/images/splits_figure.png" alt="This techniques work by driving the expression of target transgenes at the intersection between the expression patterns of two hemi-driver transgenes." max-width="50%" >

We use programmatic methods to generate expression statements for hemi-driver combinations with [FlyLight](https://www.janelia.org/project-team/flylight) image data hosted by [VFB](https://virtualflybrain.org). Combinations are validated against a local copy of the FlyLight dataset and a structured user readable comment is generated as part of the expression statement. These hyperlink to the partner hemi-driver in [FlyBase](https://flybase.org/), contain the strain designation (where available) and can be automatically parsed by [Virtual Fly Brain](](https://virtualflybrain.org)) to attach expression and genetic data to a node representing the intersection.

<img src="/images/split_vfb.png" alt="split expression shown in Virtual Fly Brain (VFB)" max-width="50%" >
