# 🩺 Skin Cancer Detection – Malignant vs Benign

This project explores the use of deep learning and feature engineering techniques for classifying dermoscopic images of skin lesions as malignant or benign, using the **ISIC dataset**.

## Overview

The main goal was to evaluate the performance of several CNN architectures in the task of binary image classification, and to understand how image preprocessing and feature transformation affect model performance.

### Models Used
- **ResNet50**
- **DenseNet121**
- **VGG16**
- **InceptionV3**

### Feature Engineering Techniques
- **CLAHE (Contrast Limited Adaptive Histogram Equalization):**  
  Enhanced image contrast to highlight critical visual structures.
- **Polynomial Feature Transformation:**  
  Introduced non-linear feature interactions by squaring extracted feature vectors.

Each model was tested under the following conditions:
- With **CLAHE** only
- With **Polynomial Transformation** only
- With **both methods combined**

## Key Result

- The best performance was achieved using **ResNet50 with CLAHE**, reaching a classification accuracy of **89%**.

This result shows that appropriate image enhancement techniques can significantly improve model performance. The project also emphasizes the importance of validating the impact of each transformation method individually and in combination.


## Instructions for Running the Project

## 1. Code Organization

- The codes for **ResNet50**, **DenseNet121**,**Inception V3** and **VGG16** are located in the **main folder**.
- There is an additional folder containing:
  - The corresponding results for each model with its combination (CLAHE, Polynomial Transformation and CLAHE + Polynomial Transformation).

## 2. Execution Order

- You should run the codes located in the **main folder**.
- The recommended order for execution is:
  1. CLAHE_Polynomial_Resnet50.ipynb
  2. CLAHE_Polynomial_DenseNet121_VGG16.ipynb
  3. InceptionV3_model.ipynb

## 3. Feature Engineering Combinations

- For each combination of feature engineering techniques:
  - **Only comment out** the lines corresponding to the functions that are **not** going to be used.
  - Leave active only the necessary preprocessing functions.
  - The code itself runs the combination CLAHE + Polynomial Transformation.

## 4. Runtime Environment

- The project must be executed in **Google Colab**.
- Check you are using a **T4 GPU**.  
- Once the notebook is loaded, simply **press "Runtime" > **"Run all"** to execute all cells in order without manual intervention.
