# MasterThesis
Code material

Alzheimer's Disease MRI Classification Using Deep Learning

This repository contains all the code and models used in our master's thesis project on classifying Alzheimer's disease stages from brain MRI images using deep learning techniques. The goal is to compare different approaches and evaluate their performance in terms of accuracy, sensitivity, specificity, F1 score, and explainability.


# The code is organized into three main .py files:
1. baseline_vgg19.ipynb
This notebook implements the baseline model using the VGG19 architecture pretrained on ImageNet. The pipeline includes:
- Preprocessing of grayscale MRI images (converted to RGB)
- Data splitting (train/validation/test)
- Class weighting for imbalanced classes
- Model training, evaluation, and confusion matrix
- Basic training/validation visualization

2. sota_resnet50.ipynb
This notebook builds a state-of-the-art model using the ResNet50 architecture. It improves upon the baseline by:
- Applying data augmentation
- Using salt-and-pepper noise
- Implementing learning rate scheduling and early stopping
- Evaluating performance with additional metrics

3. novel_vit.ipynb
This notebook implements the novel approach using a Vision Transformer (ViT), also pretrained on ImageNet. It includes:
- ViT setup using PyTorch
- Salt-and-pepper noise augmentation
- Preprocessing and class balancing
- Training and evaluation
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
- Specificity  
- F1 Score  
- Confusion Matrix  
- Training vs. Validation Loss/Accuracy plots  
- Explainability (only in the novel ViT approach)


# License
This project is for academic use only as part of a Master's thesis in Business Analytics.  
If you use or adapt any part of this work, please cite appropriately.

