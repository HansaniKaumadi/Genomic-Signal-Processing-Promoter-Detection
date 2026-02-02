# 🧬 Promoter Gene Prediction using Signal Processing & Machine Learning

This project focuses on **binary classification of DNA sequences** to identify **promoter regions** using a combination of **biologically inspired feature extraction** and **machine learning**.

Instead of treating DNA purely as text, the project applies **signal processing techniques (FFT)** alongside **k-mer frequency analysis** to capture meaningful biological patterns.

---

## 📌 Project Overview

Promoter regions play a crucial role in **gene regulation**, controlling the initiation of transcription. Accurately identifying promoter sequences is a key task in **computational biology and bioinformatics**.

In this project:
- DNA sequences are numerically encoded
- Frequency-domain patterns are extracted using **Fast Fourier Transform (FFT)**
- **k-mer statistics** capture local nucleotide dependencies
- A **Logistic Regression classifier** is trained to distinguish:
  - **Promoter sequences (+)**
  - **Non-promoter sequences (−)**

---

## 📊 Dataset

**Promoter Gene Prediction Dataset (Kaggle)**  
This is the official dataset used in the project.

🔗 https://www.kaggle.com/datasets/nayanack/promoter-gene-prediction

**Key Features**
- Labeled DNA sequences
- Binary labels (`+` for promoter, `−` for non-promoter)
- Equal-length sequences
- Contains only standard nucleotides: **A, C, G, T**

---

## 🔬 Exploratory Data Analysis

Initial analysis reveals:
- Differences in **nucleotide frequency**
- Variations in **GC content**
- Distinct structural patterns across classes

<p align="center">
  <img width="841" height="393" alt="output" src="https://github.com/user-attachments/assets/9e0079d5-adaf-4e6e-8147-def443d2f180" />
</p>


These insights motivate the use of **FFT and k-mer features**.

---

## 🧠 Feature Engineering

### 🔹 DNA Numerical Encoding
Converts letters (A, C, G, T) into numeric values to enable mathematical operations.

### 🔹 FFT Feature Extraction
Fast Fourier Transform is used to convert sequences into the frequency domain, capturing periodic and structural signals.

### 🔹 k-mer Frequency Features
Counts of small subsequences (**k-mers**) are computed to quantify local patterns.

---

## 🤖 Model Training

- **Algorithm**: Logistic Regression
- **Train/Test Split**: 80% / 20% (stratified)
- **Evaluation metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC curve & AUC
  - Confusion matrix

---

## 📈 Results & Visualizations

### 🔹 Confusion Matrix
<p align="center">
  <img width="585" height="455" alt="cm" src="https://github.com/user-attachments/assets/fee358ba-c7c5-4ab9-815d-562af2fe5b9b" />
</p>

### 🔹 ROC Curve
<p align="center">
  <img width="567" height="455" alt="roc" src="https://github.com/user-attachments/assets/6761ce14-391f-4ca8-a6e0-feb02f0d6d34" />
</p>

These plots visualize classification performance and help assess model quality.

---

## 🛠️ Tech Stack

- **Python**
- **NumPy**
- **Pandas**
- **Scikit-learn**
- **Matplotlib**
- **Signal Processing (FFT)**

---


## 🚀 Future Improvements

- Try advanced models  
  - Support Vector Machines (SVM)  
  - Random Forest  
  - Gradient Boosting  

- Explore deep learning–based sequence models  
  - Convolutional Neural Networks (CNN)  
  - Recurrent Neural Networks (RNN)  
  - Transformer-based architectures  

- Hyperparameter optimization for improved performance  

- Feature selection and dimensionality reduction techniques  

- Extended evaluation using cross-validation  

---

## 🌱 Applications

- Genomic annotation pipelines  

- Gene regulation and transcription analysis  

- Bioinformatics and computational biology workflows  

- Educational resources for machine learning in biology  

## References

- Salzberg, S.L., “A Method for Identifying Promoter Regions in DNA Sequences Using Signal Processing Techniques,” *Bioinformatics*, 1991.  
- UCI Machine Learning Repository: [Promoter Gene Sequences](https://archive.ics.uci.edu/ml/datasets/Promoter+Gene+Sequences)  
- Kaggle dataset: [DNA Promoter Gene Prediction](https://www.kaggle.com/datasets/nayanack/promoter-gene-prediction)


