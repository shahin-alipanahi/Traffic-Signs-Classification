# Traffic Signs Classification (CNN)

Traffic sign classification is an essential component of autonomous vehicles and intelligent transportation systems.  
This repository contains a Jupyter notebook that implements a convolutional neural network (CNN) to classify traffic sign images and compares two preprocessing techniques to evaluate their impact on model performance.

Notebook: [`Proj_cnn.ipynb`](https://github.com/shahin-alipanahi/Traffic-Signs-Classification/blob/main/Proj_cnn.ipynb)

---

## Table of contents
- [Overview](#overview)  
- [Key Features](#key-features)  
- [Notebook structure](#notebook-structure)  
- [Data](#data)  
- [Preprocessing techniques](#preprocessing-techniques)  
- [Model architecture](#model-architecture)  
- [Training & evaluation](#training--evaluation)  
- [How to run](#how-to-run)  
- [Requirements](#requirements)  
- [Results & visualizations](#results--visualizations)  
- [Contributing](#contributing)  
- [License & Contact](#license--contact)

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
- Clean, documented Jupyter notebook (`Proj_cnn.ipynb`) with end-to-end pipeline.
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
The notebook expects a kaggle image dataset of traffic signs: 
