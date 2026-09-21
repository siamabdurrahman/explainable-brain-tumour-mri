# Explainable Brain Tumour Classification from MRI

An academic deep-learning project for binary brain MRI classification using convolutional neural networks, transfer learning, and Grad-CAM visual explanations.

![Python](https://img.shields.io/badge/Python-3.x-3776AB)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN%20%7C%20Transfer%20Learning-6f42c1)
![Status](https://img.shields.io/badge/Status-Academic%20Prototype-0969da)

## Project objective

The project explores an end-to-end workflow for distinguishing tumour-positive and non-tumour MRI images. It combines dataset auditing, preprocessing, model development, performance evaluation, and post-hoc explainability.

## Research workflow

```text
MRI images
  -> dataset audit and class inspection
  -> preprocessing and augmentation
  -> CNN and transfer-learning experiments
  -> classification evaluation
  -> Grad-CAM visual explanations
```

## Repository contents

| File | Purpose |
| --- | --- |
| `Brain_Tumour_Detection_from_MRI_Images_Using_Convolutional_Neural_Networks_and_Transfer_Learning_(Final_Version).ipynb` | Structured final workflow |
| `Brain_tumour_classification.ipynb` | Exploratory prototype and development record |
| `Flowchart.png` | Visual overview of the experimental pipeline |
| `Dataset` | Dataset reference used by the notebooks |

The two notebooks are retained deliberately: the exploratory version shows the development process, while the final version presents the organised pipeline.

## Methods demonstrated

- Image-data auditing and preprocessing
- Convolutional neural networks
- Transfer learning
- Classification metrics and error analysis
- Grad-CAM explainability
- Reproducible notebook-based experimentation

## Running the project

1. Open the final notebook in Google Colab or Jupyter.
2. Configure the dataset location referenced in the notebook.
3. Run the audit and preprocessing cells before training.
4. Execute the evaluation and Grad-CAM sections after model training.

Hardware acceleration is recommended for deep-learning experiments. Exact package requirements and dataset access conditions should be checked in the notebook before execution.

## Responsible-use statement

This is an academic research prototype, not a medical device or clinical decision-support system. It has not been clinically validated. Predictions and heatmaps must not be used for diagnosis or patient care, and apparent Grad-CAM relevance should not be interpreted as causal clinical evidence.

## Author

**Abdur Rahman Siam**  
MSc Cybersecurity Technology researcher working across explainable AI, digital health, multimodal sensing, privacy-preserving machine learning, and IoT security.

- [ORCID](https://orcid.org/0009-0002-5904-9477)
- [LinkedIn](https://www.linkedin.com/in/abdur-rahman-siam-86a705353)
