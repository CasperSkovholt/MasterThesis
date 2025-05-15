# MasterThesis
Code material

Alzheimer's Disease MRI Classification Using Deep Learning

This repository contains all the code and models used in our master's thesis project on classifying Alzheimer's disease stages from brain MRI images using deep learning techniques. The goal is to compare different approaches and evaluate their performance in terms of accuracy, sensitivity, specificity, F1 score, and explainability.


# The code is organized into three main .py files:
1. baseline.py
This notebook implements the baseline model using the VGG19 architecture pretrained on ImageNet.

2. sota.py
This notebook builds a state-of-the-art model using the ResNet50 architecture. 

3. novel.py
This notebook implements the novel approach using a Vision Transformer (ViT), also pretrained on ImageNet. It includes:
- ViT setup using PyTorch
- Integration of XAI (LIME) for model explainability
  

# Dataset
The dataset consists of MRI images of brains classified into four stages:
- Non Demented  
- Very Mild Dementia  
- Mild Dementia  
- Moderate Dementia  

It was obtained from Kaggle: [Alzheimer MRI Dataset](https://www.kaggle.com/datasets/ninadaithal/imagesoasis/data?select=Data)
[Accessed: 9 May 2025]


# Evaluation Metrics
Each model is evaluated based on:
- Accuracy  
- Sensitivity (Recall)
- F1 Score  
- Confusion Matrix  
- Training vs. Validation Loss/Accuracy plots  
- Explainability (only in the novel ViT approach)


# License
This project is for academic use only as part of a Master's thesis in Business Analytics.  
If you use or adapt any part of this work, please cite appropriately.

