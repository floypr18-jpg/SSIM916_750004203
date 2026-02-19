# SSIM916_750004203

# Problem Set 1 – Predicting Conversions in Performance Marketing Using Classification Models

This project predicts customer conversion using a digital marketing campaign dataset.  
Two models are compared: **Logistic Regression** and **Random Forest**.

Developed and tested on macOS using Python 3.13.9 (Anaconda) and scikit-learn 1.7.2.

---

## Repository Structure

- `analysis.ipynb` — Main notebook containing full analysis pipeline  
- `data/digital_marketing_campaign_dataset.csv` — Dataset  
- `requirements.txt` — Required Python packages  

---

## Dataset

The dataset is sourced from Kaggle:

Rabie El Kharoua (2024). *Predict Conversion in Digital Marketing Dataset.*

Kaggle link:  
https://www.kaggle.com/datasets/rabieelkharoua/predict-conversion-in-digital-marketing-dataset

The dataset contains **8,000 observations** with a binary target variable `Conversion`.

If the dataset file is missing:

1. Download it from Kaggle.
2. If the `data/` folder does not exist, create it in the project root directory.
3. Place the CSV file inside it as:

```
data/digital_marketing_campaign_dataset.csv
```

---

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/floypr18-jpg/SSIM916_750004203.git
cd SSIM916_750004203
```

### 2. (Optional but recommended) Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate  # Mac/Linux
```

For Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run `analysis.ipynb` from top to bottom.

---

## Expected Outputs

The notebook produces:

- Class distribution plot  
- Logistic Regression metrics (ROC-AUC, Precision, Recall, F1, Confusion Matrix)  
- Random Forest metrics (ROC-AUC, Precision, Recall, F1, Confusion Matrix)  
- ROC curve comparison plot  
- Top 10 Random Forest feature importance plot  

All results are reproducible by running the notebook sequentially.

---

## Notes

- The train–test split uses stratification with `random_state=42`.
- Random Forest uses `n_estimators=600` and `class_weight="balanced_subsample"`.
- Logistic Regression uses `class_weight="balanced"`.
- All package versions are pinned in `requirements.txt` to ensure reproducibility.
