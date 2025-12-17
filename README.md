# Genomic Signal Processing for Promoter Detection

## Project Overview

This project applies **genomic signal processing** and **machine learning techniques** to classify DNA sequences as **promoter** or **non-promoter** regions. Promoter regions are crucial in gene expression regulation, and computational detection helps accelerate genome annotation.

The workflow is as follows:
1. Numerical encoding of DNA sequences
2. Feature extraction using frequency-based and spectral methods
3. Classification using simple, interpretable machine learning models
4. Evaluation and biological interpretation

---

## Dataset

- **Source:** [Kaggle: DNA Promoter Gene Prediction](https://www.kaggle.com/datasets/nayanack/promoter-gene-prediction)  
- **File:** `promoters.data`  
- **Description:**  
  - Labels: `+1` = promoter, `-1` = non-promoter  
  - Sequence length: 57 base pairs  
  - Includes sequence IDs for reference

> Note: This dataset is a mirror of the classic UCI Promoter Gene Sequences dataset.

---



## Methodology

1. **Data Loading & Preprocessing**  
   - Clean DNA sequences  
   - Map labels to 0 (non-promoter) and 1 (promoter)

2. **Numerical Encoding**  
   - **One-hot encoding:** Preserves nucleotide identity  
   - **EIIP encoding:** Converts nucleotides to numerical values for spectral analysis

3. **Feature Extraction**  
   - **k-mer frequency counts** (2-mer or 3-mer)  
   - **Spectral analysis:** Fast Fourier Transform (FFT) to capture periodicity patterns

4. **Machine Learning**  
   - Models used: Logistic Regression, SVM, Random Forest  
   - Train-test split or k-fold cross-validation for evaluation

5. **Evaluation Metrics**  
   - Accuracy, Precision, Recall, Sensitivity, Specificity, ROC-AUC

6. **Biological Interpretation**  
   - Identify motifs, 3-base periodicity, GC content  
   - Discuss relevance to promoter function

---

## Tools & Libraries

- Python 3.x  
- NumPy, Pandas  
- SciPy (FFT)  
- scikit-learn (classification & metrics)  
- matplotlib / seaborn (visualization)  

---



## References

- Salzberg, S.L., “A Method for Identifying Promoter Regions in DNA Sequences Using Signal Processing Techniques,” *Bioinformatics*, 1991.  
- UCI Machine Learning Repository: [Promoter Gene Sequences](https://archive.ics.uci.edu/ml/datasets/Promoter+Gene+Sequences)  
- Kaggle dataset: [DNA Promoter Gene Prediction](https://www.kaggle.com/datasets/nayanack/promoter-gene-prediction)


