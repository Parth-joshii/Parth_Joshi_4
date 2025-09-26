# 🩺 Logistic Regression on Breast Cancer Wisconsin Dataset

## 📌 Overview
This project applies **Logistic Regression** to the [Breast Cancer Wisconsin dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data).  
The task is to classify tumors as **Malignant (cancerous)** or **Benign (non-cancerous)** based on 30 medical features.

---

## 📂 Dataset
- **Source**: UCI ML Repository (via Kaggle).  
- **Target variable**: `diagnosis`  
  - `M` → Malignant (**1**)  
  - `B` → Benign (**0**)  
- **Features**: 30 numeric features describing cell nuclei characteristics.  

---

## ⚙️ Workflow
1. **Load dataset** using [KaggleHub](https://pypi.org/project/kagglehub/).  
2. **Preprocess**:
   - Drop unnecessary columns (`id`, `Unnamed: 32`).  
   - Encode diagnosis (`M=1`, `B=0`).  
3. **Train/Test Split** (80/20).  
4. **Standardize Features** with `StandardScaler`.  
5. **Train Logistic Regression Model**.  
6. **Evaluate Model**:
   - Confusion Matrix  
   - Precision, Recall, Accuracy  
   - ROC-AUC & ROC Curve Plot  
7. **Threshold Tuning** (compare default `0.5` vs custom `0.3`).  
8. **Visualize Sigmoid Function**.  

---

## 📊 Example Results
(Default threshold = 0.5)

- **Accuracy**: ~95%  
- **Precision**: ~94%  
- **Recall**: ~97%  
- **ROC-AUC**: ~0.99  

At **threshold = 0.3**, recall increases (fewer missed cancers) but precision decreases (more false positives).

---

## 📈 Visualizations
- ROC Curve  
- Sigmoid Function Curve  

---

## ▶️ How to Run

### 1. Clone this repo
```bash
git clone https://github.com/your-username/breast-cancer-logistic-regression.git
cd breast-cancer-logistic-regression
