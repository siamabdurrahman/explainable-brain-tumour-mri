# Model Card

## Model summary

This project compares a custom convolutional neural network with an ImageNet-pretrained MobileNetV2 model for binary classification of brain MRI images into tumour-positive and non-tumour classes. Grad-CAM is used to inspect spatial activation patterns for representative predictions.

## Intended use

The models are intended for academic study, reproducibility exercises and methodological comparison of baseline CNN and transfer-learning approaches. They are not intended for clinical deployment, diagnosis, screening, triage or treatment planning.

## Data

The archived experiment used 5,450 images, balanced between 2,725 tumour-positive and 2,725 non-tumour examples. Images were divided with a stratified 70/15/15 image-level split into 3,814 training, 818 validation and 818 test examples.

Dataset source: [Brain Tumor MRI - Yes or No](https://www.kaggle.com/datasets/mohamada2274/brain-tumor-mri-yes-or-no).

The dataset is not redistributed in this repository. Patient-level provenance, scanner diversity and external-cohort representativeness were not established in the supplied material.

## Evaluation

| Model | Accuracy | Precision | Recall | F1-score | ROC AUC |
| --- | ---: | ---: | ---: | ---: | ---: |
| Baseline CNN | 0.8032 | 0.8758 | 0.7066 | 0.7821 | 0.8919 |
| MobileNetV2 | 0.9364 | 0.9220 | 0.9535 | 0.9375 | 0.9858 |

The MobileNetV2 confusion matrix contains 376 true negatives, 33 false positives, 19 false negatives and 390 true positives on the archived test split.

## Interpretability

Grad-CAM highlights regions associated with model activations. These heatmaps are qualitative explanations and must not be interpreted as validated tumour segmentations or proof of clinically meaningful reasoning.

## Limitations

- Single public dataset and single image-level split
- No external, prospective or multi-centre validation
- No demonstrated patient-level separation
- No calibration or decision-curve analysis in the archived result set
- No expert-annotated localisation benchmark for Grad-CAM
- Potential sensitivity to scanner, preprocessing and acquisition differences

## Ethical and safety considerations

MRI data can encode demographic, acquisition and institutional biases. Any future clinical research should include documented governance, patient-level splitting, subgroup analysis, calibration, external validation, radiologist review and regulatory assessment.
