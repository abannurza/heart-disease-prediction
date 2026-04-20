# Heart Disease Prediction Using SCG and RProp Neural Network Models

This repository contains a MATLAB-based heart disease prediction project using Artificial Neural Network models. The study compares **Scaled Conjugate Gradient (SCG)** and **Resilient Backpropagation (RProp)** training algorithms on a Multilayer Perceptron (MLP) architecture to evaluate their performance in heart disease classification.

## Overview
Heart disease is one of the leading causes of mortality worldwide, making early prediction important for supporting medical decision-making. In this project, a neural network-based classification model was developed to predict heart disease using clinical data and an engineered feature called **Quantum Pattern**.

## Dataset
This project uses the **Heart Prediction (Quantum) Dataset**, which is publicly available on Kaggle:

[Heart Prediction Dataset (Quantum) - Kaggle](https://www.kaggle.com/datasets/shantanugarg274/heart-prediction-dataset-quantum)

The dataset contains clinical variables used for heart disease classification, including:
- Age
- Gender
- Blood Pressure
- Cholesterol
- Heart Rate
- Quantum Pattern

The target labels are represented as two classes:
- Heart disease indication
- No heart disease indication

To keep this repository organized and lightweight, the **raw dataset from Kaggle is not fully re-uploaded**.  
Instead, this repository includes only the **cleaned dataset** used in the MATLAB implementation and experiments.

## Research Objective
The main objective of this project is to compare the performance of two neural network training algorithms:
- **Scaled Conjugate Gradient (SCG)**
- **Resilient Backpropagation (RProp)**

The comparison was conducted to identify the more reliable model for heart disease prediction.

## Methodology
The general workflow of this project includes:
1. Data collection and preprocessing
2. Data labeling and target encoding
3. MLP model development
4. Model training using SCG and RProp
5. Performance evaluation using accuracy and ROC analysis

## Model Comparison
Two hidden node configurations were tested for comparison:
- **5 hidden nodes**
- **10 hidden nodes**

This comparison was used to observe how model complexity affects classification performance for both training algorithms.

## MATLAB Implementation
The MATLAB implementation in this project uses:
- `patternnet` for pattern recognition
- Input preprocessing:
  - `removeconstantrows`
  - `mapminmax`
- Performance function:
  - `crossentropy`

In the implementation script:
- The input data consists of **6 feature columns**
- The output targets are encoded into **2 output columns**
- One of the tested configurations uses **5 hidden nodes** with **SCG (`trainscg`)**

## Results Summary
The experimental results show that both SCG and RProp achieved good performance. However, **SCG demonstrated better generalization ability**, especially when using a simpler network architecture.

### Best Performing Model
**SCG with 5 Hidden Nodes**
- Training Accuracy: **92.3%**
- Validation Accuracy: **93.6%**
- Testing Accuracy: **92.3%**

### Additional Findings
- SCG performed best with **5 hidden nodes**
- RProp showed better performance at **10 hidden nodes** compared to 5 hidden nodes
- Overall, SCG was more reliable for this heart disease prediction task

## Conclusion
This project shows that **Scaled Conjugate Gradient (SCG)** is a strong and reliable training algorithm for heart disease prediction using an MLP model. Compared with RProp, SCG provided better generalization performance on unseen data in this study.

## Tools and Technologies
- MATLAB
- Artificial Neural Network (ANN)
- Multilayer Perceptron (MLP)
- SCG
- RProp
- Medical Data Analysis

## Publication
This project has been published in an IEEE conference proceeding.

**Paper Title:**  
*Heart Disease Prediction Using Scaled Conjugate Gradient and Resilient Backpropagation Neural Network Models*

**Link:**  
[View Publication on IEEE Xplore](https://ieeexplore.ieee.org/document/11470221)
