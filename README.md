# 🌞 Solar Panel Efficiency Prediction – Hackathon Project

This project was developed for a hackathon focused on predictive maintenance of solar panels using machine learning. The objective was to forecast efficiency degradation using sensor data.

---

## 📁 Dataset
- `train.csv`: 20,000 samples with 17 columns.
- `test.csv`: 12,000 samples without target.
- Provided by organizers; external data was prohibited.

## 🎯 Target Variable
- `efficiency` – represents the final energy output efficiency of each panel.

---

## 📊 Features Used
We engineered several new features:
- `temp_diff` – temperature difference between panel and ambient.
- `irradiance_per_humidity` – irradiance normalized by humidity.
- `age_squared` – to model non-linear degradation.
- `wind_pressure_ratio` – cooling effect indicator.
- `cloud_irradiance` – cloud’s impact on irradiance.

---

## 🤖 Model
- Model: **LightGBM Regressor**
- Evaluation Metric: `100 * (1 - RMSE)`
- Validation Score: **89.27**

---

## 🧠 Tools & Libraries
- Python, Pandas, Scikit-learn, LightGBM, NumPy, Matplotlib

---

## 📄 Files
- `submission_lightgbm.csv` – Prediction results
- `model_script.py` – Model training and prediction
- `approach.txt` – Summary of approach
