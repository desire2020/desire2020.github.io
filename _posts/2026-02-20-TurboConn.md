---
layout:   research
title:    Turbo Connection&#58; Reasoning as Information Flow from Higher to Lower Layers
category: publications
date:     2026-02-20
summary:  "Turbo Connection routes higher-layer states at one token to lower layers at the next, extending the effective computational path available for multi-step reasoning."
---

## Authors

Mohan Tang and **Sidi Lu**

## Context

This project was led by my student Mohan Tang, whom I mentored during my time at Tencent AI Lab Seattle.

## Overview

Turbo Connection, or TurboConn, modifies a Transformer's residual pathways so that higher-layer hidden states at token *t* can flow into lower layers at token *t + 1*. This creates a deeper effective computation path across generated tokens without requiring the full model to be trained again from scratch.

The work also studies connection density: dense routing between layers performs better than sparse alternatives that pass only a single hidden state or vector.

## Results

Fine-tuning pretrained language models with TurboConn improves accuracy by 0.9 to more than 10 percentage points on GSM8K, Parity, and multi-step arithmetic. On the Parity task, it raises a fine-tuned Qwen3-1.7B model from 53.78% to 100% accuracy, with negligible impact on generation latency.

## Paper

[arXiv](https://arxiv.org/abs/2602.17993)

## Status

Preprint, 2026.

## Citation

Mohan Tang and Sidi Lu. “Turbo Connection: Reasoning as Information Flow from Higher to Lower Layers.” arXiv:2602.17993, 2026.
