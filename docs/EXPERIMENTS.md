# Experiment and split metadata

The fixed mixed split used by the recorded run is:

| source | train | test |
|---|---:|---:|
| LOL-v2 Synthetic | 900 | 100 |
| UIEB paired subset | 800 | 90 |
| BAID subset | 301 | 67 |
| **Total** | **2,001** | **257** |

The split files contain filenames only; no images are redistributed. The
source datasets do not provide a common scene identifier, so the manifests
document file-level separation rather than making an unsupported scene-level
claim.

## Implementation status

The core PUIE network source is withheld in this review snapshot. The complete
source package is maintained separately and will be released after review.
