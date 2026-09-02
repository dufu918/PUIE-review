# PUIE: Physically Inspired Unified Enhancement

This is the anonymous review snapshot for the three-task image-enhancement
experiments (low-light, backlit and underwater). It contains the experiment
metadata, configurations and dataset-free filename manifests. The core network
implementation is intentionally withheld during review while the code is
being cleaned and organized. The complete implementation will be added after
the review/organization phase.

## Experiment record

The recorded mixed benchmark contains 2,001 training pairs and 257 test pairs:

| subset | train | test |
|---|---:|---:|
| LOL-v2 Synthetic | 900 | 100 |
| UIEB | 800 | 90 |
| BAID subset | 301 | 67 |

Training used 128×128 random crops, batch size 8, Adam with learning rate
2e-4, and 150,000 iterations. The released run optimized the Charbonnier
reconstruction loss with ε=1e-3.

## Repository status statement

> The implementation is currently being cleaned and anonymized for release.
> The present repository provides the experiment protocol and split metadata;
> the core model source and trained weights will be added after the review
> period.

No image data, checkpoints, logs, TensorBoard files or user-specific paths are
included in this snapshot. Dataset licenses and download instructions are
listed in `docs/EXPERIMENTS.md`.
