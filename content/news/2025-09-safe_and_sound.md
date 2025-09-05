---
title: "Safe & Sound: toward a community standard for acoustic metadata"
date: 2025-09-04
draft: false
description: "A quick look at the Safe & Sound effort to make bioacoustic datasets easier to share, validate, and reuse."
author: "Benjamin Cretois"
categories: ["Standards", "Data"]
tags: ["metadata", "FAIR", "PAM", "standardisation"]
---

If you’ve tried to merge acoustic datasets from different projects, you know the pain: inconsistent folder structures, missing device settings, ambiguous timestamps, and no record of which model version produced which detections. **Safe & Sound** is a community effort on WILDLABS that tackles this head-on by proposing a practical standard for **bioacoustic data and metadata**.

**What it is.** Safe & Sound is drafting a lightweight, project-level standard that covers how to organise recordings and what metadata to include so datasets are **interoperable and FAIR**. The group is aligning with existing practice rather than reinventing the wheel—for example, exploring how to **extend Camtrap DP** (widely used in camera-trap workflows) to also describe **passive acoustic monitoring (PAM)** data. The goal is a format that’s simple enough for field teams, but structured enough for downstream tooling, validation, and archiving.

**What it captures.** The draft focuses on essentials most of us already collect but rarely package consistently:
- project/site/deployment context (who, where, when, why)
- recorder + microphone configuration (model, gain, sampling rate, channels, calibration)
- file-level metadata (time zone, clock behaviour, compression)
- processing lineage (software + model versions, parameters)
- annotation and detection outputs with uncertainty and provenance

**Why it matters.** Standardised metadata de-risks long-term monitoring: it preserves effort, lets models be compared or re-run, and makes sharing with partners and repositories straightforward. For **TABMON**, adopting a common structure will speed data exchange across countries and help us publish transparent indicators with clear provenance.

**How to engage.** The Safe & Sound team is actively seeking use cases and comments on the proposed approach via the WILDLABS discussion. If your workflows already impose a structure, contribute examples—especially for edge cases (e.g., fragmented files, bat ultrasonic sampling, streaming recorders).

**Related work.** The initiative sits alongside other community standards (e.g., Open Ecoacoustics’ metadata guidance) and established schemas from adjacent domains (e.g., Tethys for marine bioacoustics). Convergence is the point: pick something usable, document it, and stick to it.

*Bottom line:* this is a pragmatic move from ad-hoc spreadsheets toward consistent, machine-readable acoustic datasets. We’ll track Safe & Sound’s progress and align TABMON’s public releases accordingly.
