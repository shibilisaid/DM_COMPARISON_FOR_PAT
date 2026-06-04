# DM_COMPARISON_FOR_PAT

This study systematically compares denoising diffusion probabilistic models (DDPM), denoising diffusion implicit models (DDIM), and score-based models for photoacoustic tomography (PAT) reconstruction across challenging limited-view scenarios.
This work utilized publicly available diffusion model implementations as the basis for the model architecture.

The DDPM and DDIM frameworks adopted in this work are based on the implementations as provided in https://github.com/hojonathanho/diffusion and https://github.com/ermongroup/ddim/tree/main
The score-based diffusion model implementation follows the methodology as in https://github.com/sreemanti-dey/diffusion\_for\_PAT


###### **Dataset**


The datasets used in this study are publicly available. The synthetic photoacoustic dataset can be obtained from:  https://github.com/sreemanti-dey/diffusion\_for\_PAT

The anatomical breast images are available from Radiopaedia: https://radiopaedia.org/articles/breast-imaging-reporting-and-data-system-bi-rads-2. The cases utilized in this study are: Case 2 (BI-RADS 4), Case 3 (BI-RADS 5), Case 5 (BI-RADS 5)  and Case 9 (BI-RADS 4)



###### **Reconstruction**



The implementation of the reconstruction algorithm of DDPM and DDIM sampling strategies, is provided in **DDPM\_PAT.ipynb** and **DDIM\_PAT.ipynb**, respectively. These notebooks contain the complete workflow, including data processing, model training and inverse problem reconstruction.



