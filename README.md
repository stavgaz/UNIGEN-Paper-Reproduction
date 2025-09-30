# UNIGEN Reproduction Study

This repository contains a reproduction of the paper:

**UNIGEN: Universal Domain Generalization for Sentiment Classification
via Zero-shot Dataset Generation**\
*(Choi et al., EMNLP 2024)*

Conducted at the **National Technical University of Athens (NTUA)**,
DSML (Data Science and Machine Learning), 2024-25.\
Author: **Stavros Gazetas** (stavrosgazetas@mail.ntua.gr)

------------------------------------------------------------------------

## Overview

UNIGEN is a framework for **zero-shot dataset generation** that enables
training lightweight **Task-Specific Models (TAMs)** for sentiment
classification without annotated domain-specific data.

This work reproduces the original study under **resource constraints**,
using GPT-2 Large (774M parameters) instead of GPT-2 XL, and generating
**20k synthetic samples** instead of 1M.

------------------------------------------------------------------------

## Method

-   Universal dataset generation with a domain-agnostic prompt
-   Noise reduction via **soft relabeling**, **denoising memory bank**,
    and **supervised contrastive learning**
-   Evaluation with multiple TAMs: **LSTM, CNN, DistilBERT, RoBERTa,
    TinyBERT**

------------------------------------------------------------------------

## Results

-   UNIGEN demonstrated strong **cross-domain generalization** even at
    smaller scale
-   **DistilBERT and RoBERTa** TAMs were competitive with or superior to
    baselines (ZEROGEN, SUNGEN)
-   **TinyBERT** showed promising results under limited resources
-   **LSTM and TextCNN** underperformed, confirming the importance of
    pretrained models

------------------------------------------------------------------------

## Citation

If you use this work, please cite the original paper:

> Choi, J., Kim, H., Park, S., & Moon, H. (2024). **UNIGEN: Universal
> Domain Generalization for Sentiment Classification via Zero-shot
> Dataset Generation.** *Proceedings of EMNLP 2024.*
