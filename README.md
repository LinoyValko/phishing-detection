# Phishing Detection – Machine Learning Preprocessing Pipeline
---

## Project Description

This project focuses on building a robust **data preprocessing pipeline** for a phishing website detection task.  
The pipeline prepares the data for machine learning classification by applying various preprocessing steps such as:

- Missing value handling
- Label encoding & one-hot encoding
- Feature scaling
- Train-test split
- Feature selection (e.g., mutual information)
- Pipeline construction using `sklearn.pipeline`

---

## Dataset Overview

- Filename: `Phishing_Legitimate_full.csv`
- Number of samples: ~11,000
- Target variable: `CLASS_LABEL`  
  - 0 = Legitimate website  
  - 1 = Phishing website
- Feature types:  
  - Categorical (URLs, protocols, domains, etc.)  
  - Numerical (lengths, entropy, etc.)

---

## Pipeline Highlights

- **Missing Values**: Filled with mean/most frequent depending on feature type
- **Label Encoding**: For binary categorical features
- **One-Hot Encoding**: For multi-class categorical features
- **Scaling**: StandardScaler used for numeric columns
- **Feature Selection**: Top K features selected using mutual information
- **Final Pipeline**: Built using `ColumnTransformer` and `Pipeline` from `sklearn`

---

## How to Run

1. Clone this repository or download the files
2. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn


