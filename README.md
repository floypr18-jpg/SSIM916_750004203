# SSIM916_750004203

# Problem Set 1 – Predicting Conversions in Performance Marketing Using Classification Models

This project predicts customer conversion using a digital marketing campaign dataset.
Two models are compared: Logistic Regression and Random Forest.

Developed and tested on macOS using Python 3.13.9 (Anaconda) and scikit-learn 1.7.2.

---

## Repository Structure

- analysis.ipynb — Main notebook containing full analysis pipeline
- data/digital_marketing_campaign_dataset.csv — Dataset
- requirements.txt — Required Python packages

---

## Setup Instructions

1. Clone the repository:

   git clone <your-repo-link>
   cd SSIM916_750004203

2. (Optional but recommended) Create a virtual environment:

   python -m venv venv
   source venv/bin/activate  (Mac/Linux)
   venv\Scripts\activate     (Windows)

3. Install dependencies:

   pip install -r requirements.txt

4. Open Jupyter Notebook:

   jupyter notebook

5. Run analysis.ipynb from top to bottom.

---

## Expected Outputs

The notebook produces:

- Class distribution plot
- Logistic Regression metrics (ROC-AUC, Precision, Recall, F1, Confusion Matrix)
- Random Forest metrics (ROC-AUC, Precision, Recall, F1, Confusion Matrix)
- ROC curve comparison plot
- Top 10 Random Forest feature importance plot

---

## Notes

- Random seed is fixed at 42 for reproducibility.
- All package versions are pinned in requirements.txt to ensure reproducibility.
