# PUIE

This repository accompanies the paper **“PUIE: A Physically Inspired Unified
Framework for Image Enhancement Under Complex Illumination.”** PUIE is a
unified model for low-light, backlit and underwater image enhancement.

## Repository status

The current release contains the experiment configurations and the filename
lists used to construct the mixed benchmark. The model implementation and
pretrained weights are being organized and will be included in a subsequent
release.

## Experimental setup

The mixed benchmark release contains 2,000 training pairs and 257 test pairs:

| Subset | Train | Test |
|---|---:|---:|
| LOL-v2 Synthetic | 900 | 100 |
| UIEB | 800 | 90 |
| BAID subset | 300 | 67 |

Training used 128×128 random crops, a batch size of 8, Adam with a learning
rate of 2×10⁻⁴, and 150,000 iterations. The recorded run used the Charbonnier
reconstruction loss with ε=10⁻³.

## Contents

- `configs/` — main experiment configuration;
- `splits/` — dataset-free filename lists for the mixed benchmark;
- `docs/` — additional experiment and split information.

The datasets, checkpoints and experiment outputs are not distributed with
this repository. Please obtain the datasets from their original sources and
follow the corresponding licenses.
