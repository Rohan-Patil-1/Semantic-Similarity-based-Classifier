# Visual-Semantic Siamese Network for Explaining Generative Lung Nodule Transformations

This repository provides the implementation and pretrained weights for a Semantic Similarity-based Siamese Convolutional Neural Network (SCNN) developed to validate and explain VAE-generated lung nodule transformations. The framework learns semantically meaningful embeddings of spiculated and non-spiculated lung nodules through structured triplet mining and metric learning.

The proposed model was trained on expert-annotated lung nodules from the LIDC-IDRI dataset and evaluated on VAE-generated latent-space transformations. The selected Siamese model achieved **81.35% accuracy**, **81.86% specificity**, and **73.43% sensitivity** during inference on reconstructed lung nodules. The framework further demonstrated progressive semantic transitions from non-spiculated to spiculated nodules, with Counterfactual Validity (CV) scores increasing from **0.012 to 0.995** across latent-space traversals.

The learned embeddings can be used for semantic validation of generative models, visual-semantic explanations, counterfactual analysis, medical image similarity learning, and explainable computer-aided diagnosis (CAD) systems.

## Repository Contents

1. **siamese_training.py**

   * Training pipeline for the Semantic Similarity-based Siamese Network. Includes metric learning, and KNN-based evaluation.

2. **siamese_model_weights.pth**

   * Pretrained Siamese Network weights used for semantic classification and explainability analysis.
  
3. **Methodology Diagram.png**

   * Proposed Methodology diagram for structured triplet mining, siamese embedding learning and explanations.

![Proposed Methodology](Methodology%20Diagram.png)

## Paper

**A Visual-Semantic Framework for Explaining Generative Lung Nodule Transformations Via Siamese Network**

Under review for publication at **IEEE eScience 2026**.

## Author(s)

### Presenter / First Author
```
Rohan Patil
DePaul University (United States)
```
### Authors

```
Charmi Patel
DePaul University (United States)

Rashi Jain
DePaul University (United States)

Yiyang Wang
Milwaukee School of Engineering (United States)

Khizer Khan
DePaul University (United States)

Roselyne Tchoua
DePaul University (United States)

Alexandru Orhean
DePaul University (United States)

Jacob Furst
DePaul University (United States)

Daniela Raicu
DePaul University (United States)
```

## Acknowledgement

This work was supported by the National Institutes of Health (NIH) through the **VS-EDGE: Visual-Semantic Explanations for Diagnostic Guidance** project under award number **1R15CA297521-01**.

## Dataset

* Lung Image Database Consortium and Image Database Resource Initiative (LIDC-IDRI) - ```https://www.cancerimagingarchive.net/collection/lidc-idri/```

## Applications

* Explainable Medical AI
* Metric Learning for Medical Imaging
* VAE Latent-Space Validation
