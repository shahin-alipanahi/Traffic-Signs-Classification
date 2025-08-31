# Traffic Signs Classification using Convolutional Neural Networks(CNN) 

Traffic sign classification is an essential component of autonomous vehicles and intelligent transportation systems.  
This repository contains a Jupyter notebook that implements a convolutional neural network (CNN) to classify traffic sign images and compares two preprocessing techniques to evaluate their impact on model performance.


---

## Table of contents
- [Overview](#overview)  
- [Key Features](#key-features)  
- [Notebook structure](#notebook-structure)  
- [Data](#data)  
- [Preprocessing techniques](#preprocessing-techniques)  
- [Model architecture](#model-architecture)  
- [Training & evaluation](#training--evaluation)  

---

## Overview
This project implements and evaluates a convolutional neural network for traffic sign classification. The notebook walks through:
- loading and inspecting the dataset,
- applying two different preprocessing pipelines,
- designing and training a CNN,
- comparing model performance across preprocessing methods using metrics and visualizations (accuracy curves, confusion matrix, classification report).

The main aim is to demonstrate how preprocessing choices affect classification accuracy and to present clear experimental results.

---

## Key Features
- Documented Jupyter notebook with end-to-end pipeline.
- Comparison of two preprocessing approaches and their effect on model performance.
- Standard training / validation split, metrics (accuracy, precision, recall, F1), and visualizations.
- Instructions to reproduce experiments locally.

---

## Notebook structure
The notebook is organized into sections (typical ordering):
1. Imports & setup — library imports and configuration.  
2. Dataset loading & exploration — sample images, class distribution.  
3. Preprocessing pipeline A — (e.g., resizing, normalization, simple augmentation).  
4. Preprocessing pipeline B — (e.g., histogram equalization / color normalization / alternative augmentation).  
5. Model definition — convolutional neural network architecture.  
6. Training — compile and train model with callbacks (checkpointing, early stopping).  
7. Evaluation — test metrics, confusion matrix, classification report.  
8. Comparison & analysis — compare the two preprocessing techniques and discuss results.  

---

## Data
The notebook expects a kaggle image dataset of traffic signs: [valentynsichkar/traffic-signs-preprocessed](https://www.kaggle.com/datasets/valentynsichkar/traffic-signs-preprocessed)

Adjust paths inside the notebook as needed.

---

## Preprocessing techniques
This project compares two preprocessing approaches (implemented and evaluated in the notebook). Examples of preprocessing steps:
- Pipeline A (Baseline): Resize images → convert to RGB → scale pixel values (0–1) → basic augmentations (flip, rotate).  
- Pipeline B (Enhanced): Resize → contrast/histogram equalization or CLAHE → color normalization → more aggressive augmentation.  

The notebook contains the exact implementations and code to switch between these pipelines during training.

---

## Model architecture
A straightforward CNN is implemented in the notebook (Conv → ReLU → Pool → Dropout → Dense). The notebook includes:
- layer-by-layer model definition,
- model.summary(),
- parameter counts and rationale for design choices.

---

## Training & evaluation
- Loss: categorical crossentropy  
- Optimizer: Adam  
- Metrics: accuracy, precision, recall, F1  
- Visualization: training/validation curves, confusion matrix, classification report, sample predictions  

Early stopping and model checkpointing are included to prevent overfitting.

---

## How to run
1. Clone the repository:
   ```bash
   git clone https://github.com/shahin-alipanahi/Traffic-Signs-Classification.git
   cd Traffic-Signs-Classification
   ```
   
## Install Dependencies 
```bash
 pip install -r requirements.txt
   ```
