# Skin-Cancer-Classification-Deep-Learning-Project

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
- It is mandatory to use a **T4 GPU** for consistency.  
- Once the notebook is loaded, simply **press "Runtime" > **"Run all"** to execute all cells in order without manual intervention.
