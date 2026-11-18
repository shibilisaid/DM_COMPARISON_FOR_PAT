# Diffusion Model Comparison for Photoacoustic Tomography (PAT)

**Repository:** `DM_COMPARISON_FOR_PAT`

## Overview

This project investigates and compares three diffusion-based approaches for **photoacoustic tomography (PAT) image reconstruction** under challenging limited-view acquisition conditions:

- **Denoising Diffusion Probabilistic Models (DDPM)**
- **Denoising Diffusion Implicit Models (DDIM)**
- **Score-based diffusion models**

The study builds on publicly available diffusion-model implementations and prior work on score-based PAT reconstruction. The objective is to examine the application of these approaches to limited-view PAT inverse problems.

## Datasets

### Synthetic photoacoustic data

The synthetic PAT dataset is available through the repository accompanying the score-based PAT reconstruction study:

- [Score-Based Diffusion Models for PAT — datasets and code](https://github.com/sreemanti-dey/diffusion_for_PAT)

### Anatomical breast images

Anatomical breast images used in this study were obtained from **Radiopaedia**. The cases considered in the study are identified as follows:

| Case | BI-RADS category |
| --- | --- |
| Case 2 | BI-RADS 4 |
| Case 3 | BI-RADS 5 |
| Case 5 | BI-RADS 5 |
| Case 9 | BI-RADS 4 |

- [Radiopaedia: Breast Imaging Reporting and Data System (BI-RADS)](https://radiopaedia.org/articles/breast-imaging-reporting-and-data-system-bi-rads-2)

**Note:** The Radiopaedia link above is a BI-RADS reference page, not a direct link to the individual cases. Case-specific source links should be added where available. Please consult the original sources for applicable reuse and attribution requirements.

## Reconstruction notebooks

| Notebook | Description |
| --- | --- |
| [`DDPM_PAT.ipynb`](DDPM_PAT.ipynb) | DDPM-based PAT workflow, including data processing, model training, and inverse-problem reconstruction. |
| [`DDIM_PAT.ipynb`](DDIM_PAT.ipynb) | DDIM-based PAT workflow, including data processing, model training, and inverse-problem reconstruction. |

The score-based approach is based on the methodology described in the [score-based PAT project](https://github.com/sreemanti-dey/diffusion_for_PAT). Its implementation details are available from that source; no local score-based notebook is specified here.

## Getting started

1. Download or clone this repository.
2. Obtain the datasets from the sources linked above, subject to their usage terms.
3. Open the relevant notebook in Jupyter Notebook or JupyterLab.
4. Install the packages imported by the notebook and update dataset and output paths for your environment.
5. Execute the notebook cells in order to run the data-processing, training, and reconstruction workflow.

**Reproducibility note:** Exact package versions, hardware requirements, dataset directory layouts, trained checkpoints, and run settings have not been specified in this README. Consult the notebook code before attempting to reproduce the experiments.

## Original implementations and references

This study uses the following publicly available work as methodological or implementation references:

1. **DDPM:** Ho, J., Jain, A., & Abbeel, P. (2020). *Denoising Diffusion Probabilistic Models*. [Paper](https://arxiv.org/abs/2006.11239) · [Official code](https://github.com/hojonathanho/diffusion)
2. **DDIM:** Song, J., Meng, C., & Ermon, S. (2021). *Denoising Diffusion Implicit Models*. [Paper](https://arxiv.org/abs/2010.02502) · [Official code](https://github.com/ermongroup/ddim)
3. **Score-based PAT:** Dey, S., et al. (2024). *Score-Based Diffusion Models for Photoacoustic Tomography Image Reconstruction*. ICASSP 2024. [Project code and data](https://github.com/sreemanti-dey/diffusion_for_PAT)

## Acknowledgments and usage

We acknowledge the authors of the original DDPM, DDIM, and score-based PAT implementations, as well as Radiopaedia and the contributors of the datasets used in this study. These resources remain the work of their respective creators. When reusing code or data, consult and comply with the applicable licenses, citation requirements, and terms of use from each original source.




## Citation

If you use this repository, its implementation, or the associated
research findings in your work, please cite our published paper:

**Said, S., & Barhumi, I. (2026).** A comparative study of
diffusion-based reconstruction frameworks for photoacoustic
tomography. *Scientific Reports, 16*, Article 27361.

**Paper:** https://doi.org/10.1038/s41598-026-57923-2

### BibTeX

```bibtex
@article{Said2026PAT,
  author  = {Said, Shibili and Barhumi, Imad},
  title   = {A comparative study of diffusion-based reconstruction
             frameworks for photoacoustic tomography},
  journal = {Scientific Reports},
  volume  = {16},
  pages   = {27361},
  year    = {2026},
  doi     = {10.1038/s41598-026-57923-2},
  url     = {https://doi.org/10.1038/s41598-026-57923-2}
}
```

