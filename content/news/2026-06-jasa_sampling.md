---
title: "Smarter annotation strategies for bird detection models — new paper in JASA"
date: 2026-06-01
draft: false
description: "A new TABMON paper published in the Journal of the Acoustical Society of America shows how to select the most valuable audio samples for annotation, drastically improving bird detection models under realistic passive acoustic monitoring conditions."
author: "Corentin Bernard"
categories: ["announcements", "AI"]
tags: ["machine-learning", "PAM", "active-learning", "data-pipeline"]
---

A new paper from the TABMON team has been published in the *Journal of the Acoustical Society of America*: **"Data-driven sampling strategies for fine-tuning bird detection models"** by Corentin Bernard, Ben McEwen, Benjamin Cretois, Hervé Glotin, Dan Stowell, and Ricard Marxer.

The full paper is freely available here: [doi.org/10.1121/10.0043947](https://pubs.aip.org/asa/jasa/article/159/6/4891/3393438/Data-driven-sampling-strategies-for-fine-tuning)

## The challenge: too much data, too few annotators

Passive acoustic monitoring produces enormous volumes of audio. Identifying bird species automatically requires fine-tuning pre-trained models like BirdNET on local recordings — but expert annotation is slow, costly, and a scarce resource. With an annotation budget covering only **0.2% of the available data** (500 samples out of ~18,000), which recordings should you label to get the biggest improvement in model performance?

This paper provides concrete, practical answers.

## Three contributions

### 1. Fighting catastrophic forgetting with L2-SP regularisation

When fine-tuning BirdNET on new local data, the model tends to "forget" species it already knew — a phenomenon called catastrophic forgetting. The authors show that a simple regularisation technique (L2-SP) that penalises large deviations from the original BirdNET weights largely prevents this, improving detection performance across 106 European bird species without any additional data.

### 2. A new "influence score" to find the most valuable samples

The core methodological contribution is the **influence score**: a data-driven measure of how much including a given audio sample in the fine-tuning set actually improves model performance. It is computed using *reverse correlation* — running thousands of random sub-selections and correlating each sample's presence/absence with the resulting model performance.

The analysis reveals that samples containing **rare species** tend to have the highest influence — intuitively, they are the ones most underrepresented and therefore most informative. Fine-tuning on the top 500 highest-influence samples achieves a cmAP of **0.456**, compared to **0.373** for random selection — a substantial gain from just a different choice of what to annotate.

Because computing influence scores requires a fully annotated dataset (impractical in the field), the authors also train a linear model on BirdNET embeddings to *predict* influence scores for unseen data, enabling practical deployment.

### 3. Practical sampling strategies: acoustic indices vs. model predictions

Finally, the paper compares a range of annotation-free and model-based strategies for selecting samples to annotate:

| Strategy | cmAP |
|---|---|
| Pre-trained BirdNET (no fine-tuning) | 0.367 |
| Random selection | 0.373 |
| Best acoustic index (TFSD threshold) | 0.394 |
| Model uncertainty (high entropy) | 0.406 |
| Predicted influence score | 0.410 |
| Oracle top influence (upper bound) | 0.456 |

**Model uncertainty** (selecting samples where BirdNET is most uncertain) emerges as the best practical strategy when model predictions are available. When they are not — for example, with unsupervised models or entirely new species — the acoustic index **TFSD** (Time-Frequency Spectral Derivation, capturing spectral modulations in the 2–10 kHz bird frequency range) is the strongest alternative and can be computed directly from raw audio with no prior annotations.

## Why it matters for TABMON

These findings directly inform how TABMON manages its annotation pipeline. The network continuously collects audio across four countries; deciding *which* recordings to send to expert annotators for labelling is a real operational constraint. The strategies validated here — particularly uncertainty sampling and TFSD-based selection — are being integrated into TABMON's active learning infrastructure to make the most of limited expert time.

The code and data used in the study are openly available:  
- GitHub: [github.com/mim-team/PAM_data_sampling](https://github.com/mim-team/PAM_data_sampling)  
- Zenodo: [zenodo.org/records/19206665](https://zenodo.org/records/19206665)
