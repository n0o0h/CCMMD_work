# Cross-Cultural Misogynistic Meme Detection (CCMMD)

## Overview

This repository contains the implementation and experimental notebooks for our research on **Cross-Cultural Multimodal Misogyny Detection (CCMMD)**. The proposed framework aims to automatically identify misogynistic memes by jointly analyzing textual and visual information across multiple languages and cultural contexts.

The framework adopts a multimodal learning approach by combining language and vision encoders with various feature fusion strategies for robust binary classification.

---

## Research Objective

Social media memes often convey harmful and misogynistic content through a combination of images and text. Traditional unimodal approaches fail to capture these cross-modal interactions effectively.

This work proposes a generalized multimodal framework that:
- Extracts semantic information from meme text.
- Extracts contextual visual features from meme images.
- Combines both modalities through multimodal fusion.
- Classifies memes as:
  - Misogynistic
  - Non-Misogynistic

---

## Supported Languages

The framework has been evaluated on:

- English
- Tamil
- Malayalam

making it suitable for both high-resource and low-resource language settings.

---

## Repository Structure

```
CCMMD_work/
│
├── codabenchenglishmisogyny.ipynb
├── codabenchtamilmisogyny.ipynb
├── codabenchmalayalammisogyny.ipynb
│
├── README.md
└── .gitignore
```

---

## Methodology

The proposed framework follows a multimodal pipeline:

```
Meme Dataset
(Image + Text)
        |
+-------+-------+
|               |
Visual      Language
Encoder      Encoder
|               |
Visual      Textual
Features    Features
+-------+-------+
        |
Multimodal Fusion
        |
Classification
        |
Prediction
```

Multiple fusion mechanisms are investigated, including:

- Concatenation
- Average Pooling
- Attention Fusion
- Gated Fusion
- Element-wise Fusion

---

## Features

- Multimodal learning
- Cross-cultural meme understanding
- Transformer-based representations
- Multiple fusion strategies
- Binary misogyny classification
- Support for multilingual datasets

---

## Experimental Notebooks

| Notebook | Description |
|----------|------------|
| English | English misogyny detection experiments |
| Tamil | Tamil misogyny detection experiments |
| Malayalam | Malayalam misogyny detection experiments |

---

## Evaluation Metrics

The framework is evaluated using standard classification metrics:

- Accuracy
- Macro F1-score
- Weighted F1-score
- Area Under ROC Curve (AUC)

---

## Requirements

Typical dependencies include:

```
Python 3.x
PyTorch
Transformers
Torchvision
NumPy
Pandas
Scikit-learn
Matplotlib
OpenCV
Pillow
```

---

## Research Contribution

This repository accompanies our research on cross-cultural multimodal misogyny detection by investigating the effectiveness of combining textual and visual representations through different multimodal fusion strategies across diverse linguistic settings.

---


---

## License

This repository is intended for research and academic purposes.
