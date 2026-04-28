# K-Nearest Neighbors (KNN)

##  Overview
This assignment applies the K-Nearest Neighbors classification algorithm on an artificial dataset to predict the **TARGET CLASS** of each data point.

---

## Files
| File | Description |
|------|-------------|
| `KNNAssignment.ipynb` | Main notebook with full solution |
| `KNN_Project_Data` | Dataset used for training and testing |

---

## Dataset
- **Rows:** 1,000 samples  
- **Features:** 10 numerical features (XVPM, GWYH, TRAT, TLLZ, IGGA, HYKR, EDFS, GUUB, MGJM, JHZC)  
- **Target:** Binary classification — `TARGET CLASS` (0 or 1)

---

## Steps Covered
1. **Import Libraries** — pandas, numpy, matplotlib, seaborn, sklearn
2. **Load Data** — Read KNN_Project_Data into a DataFrame
3. **EDA** — Pairplot with hue on TARGET CLASS
4. **Standardization** — StandardScaler applied to all features
5. **Train/Test Split** — 70% train / 30% test (random_state=101)
6. **KNN Model (K=1)** — Baseline model
7. **Evaluation** — Confusion matrix & classification report
8. **Elbow Method** — Tested K values from 1 to 39
9. **Optimal Model (K=31)** — Retrained with best K value

---

## Results

| Model | K Value | Accuracy |
|-------|---------|----------|
| Baseline | K = 1 | 72% |
| **Optimized** | **K = 31** | **84%** |

Using the elbow method, **K=31** was identified as the optimal value, reducing the error rate from **0.28** to **0.16** and significantly improving model performance over the baseline.

---

## Requirements
```
pandas
numpy
matplotlib
seaborn
scikit-learn
