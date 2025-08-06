# 🔍 Hyperparameter Tuning with KNN & SVM

This project demonstrates **hyperparameter tuning** using **GridSearchCV** and **RandomizedSearchCV** for **K-Nearest Neighbors (KNN)** and **Support Vector Machine (SVM)** classifiers.  
The goal is to optimize model parameters for the highest possible accuracy.

---

## 🛠️ Tech Stack
- **Language:** Python 3  
- **Libraries:** scikit-learn, pandas, numpy, seaborn, matplotlib  
- **Platform:** Jupyter Notebook / Google Colab  

---

## 📂 Project Structure
| File | Description |
|------|-------------|
| `GridSearchCV.ipynb` | Core notebook containing data preprocessing, model training, and parameter tuning |
| `README.md` | Project overview and documentation |

---

## 🚀 Workflow Overview

### 1️⃣ Data Preparation
- Load and explore dataset
- Separate features and target variable
- Split into training and testing sets

### 2️⃣ Model Training
- Train **KNN** classifier with a chosen value of `n_neighbors`
- Train **SVM** classifier with default parameters

### 3️⃣ Hyperparameter Tuning
#### 🔹 GridSearchCV
- Exhaustively tests all parameter combinations  
- Parameters tuned:
  - **SVM**
    - `C` : [1, 10, 20, 30]
    - `kernel` : ['rbf', 'linear']  
- Best Accuracy: **0.98** with (`C`=1, `kernel`='rbf') or (`C`=1, `kernel`='linear')

#### 🔹 RandomizedSearchCV
- Randomly samples parameter combinations for faster results  
- Parameters tuned:
  - **SVM**
    - `C` : [1, 10, 20, 30]
    - `kernel` : ['rbf', 'linear']  
- Best Accuracy: **0.98** with (`C`=10, `kernel`='rbf') or (`C`=1, `kernel`='rbf')

---

## 📊 Performance Metrics
| Model | Accuracy (Before Tuning) | Accuracy (After Tuning) |
|-------|--------------------------|--------------------------|
| KNN | 1.00 | N/A |
| SVM | 1.00 | 0.98 (Optimal params) |

---

## 📈 Example Output
- **Parameter Search Results Table** from GridSearchCV & RandomizedSearchCV  
- **Best Parameters** for highest accuracy  
- **Model Accuracy Comparison** before and after tuning

---


