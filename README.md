# Bike Sharing Rental Prediction

A machine learning project to predict daily bike rental demand using the UCI Bike Sharing dataset. Built with Python, Pandas, Scikit-learn, Matplotlib, and Seaborn.

**Student:** Nitin | **Roll No:** 2323008

---

## Project Structure

```
Bike-Sharing-Rental-Prediction/
│
├── Datasets/
│   ├── day.csv               # Raw daily bike sharing data
│   ├── hour.csv              # Raw hourly bike sharing data
│   └── final_dataset.csv     # Cleaned & preprocessed dataset
│
├── Bike_Sharing_Rental_Prediction.ipynb   # Step 1: Data Loading & Preprocessing
├── Visualisation.ipynb                    # Step 2: EDA & Visualizations
├── Prediction_models.ipynb                # Step 3: Model Building & Evaluation
├── Project_Synopsis.docx                  # Project synopsis document
└── Code_Screen_Recording.mp4             # Code walkthrough video
```

---

## Dataset

- **Source:** UCI Machine Learning Repository — Bike Sharing Dataset
- **Records:** 731 daily entries (2011–2012)
- **Target Variable:** `total_rentals` (daily bike rental count)
- **Features:** Season, Year, Month, Holiday, Working Day, Weather, Temperature, Humidity, Windspeed

---

## Workflow

### Step 1 — Data Preprocessing (`Bike_Sharing_Rental_Prediction.ipynb`)
- Load raw dataset
- Handle missing values and duplicates
- Remove leakage columns (`casual`, `registered`)
- Rename and clean columns
- Export `final_dataset.csv`

### Step 2 — EDA & Visualisation (`Visualisation.ipynb`)
- Distribution of daily rentals
- Temperature vs Rentals scatter plot
- Average rentals by season
- Working day vs holiday comparison
- Correlation heatmap

### Step 3 — Model Building (`Prediction_models.ipynb`)
- Train/Test split (80/20)
- One-hot encoding of categorical features
- Three models trained and evaluated:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
- Evaluation metrics: MAE, RMSE, R²

---

## Models & Results

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression | — | — | — |
| Decision Tree | — | — | — |
| Random Forest | — | — | ✅ Best |

> Random Forest gave the best performance with lowest error and highest R² score.

---

## Libraries Used

```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Install all dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## How to Run

1. Clone this repository
2. Install dependencies
3. Run notebooks in order:
   - `Bike_Sharing_Rental_Prediction.ipynb`
   - `Visualisation.ipynb`
   - `Prediction_models.ipynb`
