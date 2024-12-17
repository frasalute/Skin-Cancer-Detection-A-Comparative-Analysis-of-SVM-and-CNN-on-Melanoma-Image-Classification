# Skin-Cancer-Detection-A-Comparative-Analysis-of-SVM-and-CNN-on-Melanoma-Image-Classification

(Done in a university setting as project part of a Machine Learning and Deep Learning class together with other three students.)

This project implements a comparative study of **Support Vector Machines (SVM)** and **Convolutional Neural Networks (CNN)** for the classification of melanoma (benign vs malignant) using image datasets. 

## Overview
With the increasing prevalence of melanoma skin cancer, this project aims to develop reliable machine learning models to assist dermatologists in early diagnosis. The study integrates classical machine learning techniques (SVM) and deep learning methods (CNN), comparing their performance in terms of accuracy and efficiency.

## Dataset
The dataset consists of images categorized into:
- **Benign**
- **Malignant**
- **Undetected**

Dataset preprocessing involved:
1. **Filtering**: Removal of duplicates using image hashing (aHash, dHash, wHash).
2. **Aspect Ratio Filtering**: Removing images outside valid size ranges.
3. **RGB Filtering**: Ensuring proper color balance.
4. **Image Resizing**: Resized all images to 128x128 pixels for uniformity.

## Methods and Models

### 1. **Naive Bayes (Baseline)**
- Simple probabilistic classifier.
- Accuracy: **58%**.

### 2. **Support Vector Machines (SVM)**
- GridSearchCV for hyperparameter tuning.
- **Feature Selection**: Random Forest to reduce dimensions.
- **Dimensionality Reduction**: Principal Component Analysis (PCA).
- Accuracy (after optimization): **87%**.

### 3. **Convolutional Neural Networks (CNN)**
- Custom CNN architecture with:
  - 3 Convolutional Layers (ReLU activation, MaxPooling).
  - Batch Normalization.
  - Fully Connected Dense Layers with Dropout.
- Optimizer: **Adam** | Loss: **Categorical Crossentropy**
- Accuracy: **88%** on test data.

## Results
| Model        | Accuracy |
|--------------|----------|
| Naive Bayes  | 58%      |
| SVM          | 87%      |
| CNN          | **88%**  |

The CNN outperformed traditional SVM, showcasing deep learning's strength in image classification tasks.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/frasalute/Skin-Cancer-Detection-A-Comparative-Analysis-of-SVM-and-CNN-on-Melanoma-Image-Classification.git
   cd Skin-Cancer-Detection-A-Comparative-Analysis-of-SVM-and-CNN-on-Melanoma-Image-Classification
   ```
2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Running the Code
1. **Preprocessing and Filtering**:
   - Run the image filtering scripts to prepare the dataset.
2. **Naive Bayes and SVM**:
   - Execute the corresponding sections for feature selection, PCA, and SVM tuning.
3. **CNN Training**:
   - Train the CNN model using:
     ```python
     python train_cnn.py
     ```
4. **Evaluation**:
   - Evaluate the models and generate confusion matrices.

## Dependencies
- Python 3.8+
- TensorFlow 2.0+
- scikit-learn
- numpy, pandas, matplotlib, seaborn

## Key Insights
- CNN demonstrated higher accuracy and generalizability compared to SVM.
- Feature selection with Random Forest and dimensionality reduction (PCA) significantly improved SVM performance.
