# 🌫️ Air Quality in Indian Cities – Forecasting & Insights 

A machine learning project to analyze and forecast **Air Quality Index (AQI)** levels across multiple Indian cities using historical pollution data and predictive modeling. This project enables users to:
- Predict AQI for a specific **city and future year**
- View the **top 10 most polluted cities** for any year
- Visualize monthly AQI trends and categorize air quality into health-based **AQI buckets**

---

## 📌 Features

✅ Cleaned and preprocessed air pollution dataset from Indian cities  
✅ Calculates `Total Pollution` from major pollutants (PM2.5, PM10, NOx, etc.)  
✅ Trains a **Random Forest Regressor** for AQI prediction  
✅ Predicts AQI for:
- 🔍 Any selected city and year
- 🔝 Top 10 cities in a given future year  
✅ Categorizes AQI into standard **AQI buckets** (Good, Poor, Severe, etc.)  
✅ Includes interactive CLI menu and clear visualizations

---

## 📊 Dataset Information

- **Source**: Central Pollution Control Board (CPCB) via Kaggle  
- **Columns Used**:
  - `City`, `Date`, `PM2.5`, `PM10`, `NO`, `NO2`, `NOx`, `NH3`, `CO`, `SO2`, `O3`, `Benzene`, `Toluene`, `Xylene`, `AQI`
- Derived:
  - `Total Pollution` (sum of all pollutants)
  - `Year`, `Month`
  - `AQI Bucket` (classified from predicted AQI)

---

## 🧠 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn (Random Forest)
- Matplotlib
- Joblib (for saving model)

---

## ⚙️ Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/SiddardhaShayini/Air-Quality-in-Indian-Cities.git
cd Air-Quality-in-Indian-Cities
````

2. **Install dependencies**

```bash
pip install pandas numpy scikit-learn matplotlib joblib
```

3. **Run the jupyter notebook**

---

## 🧪 Sample Usage

```
📋 Select Option:
1. Predict AQI for a Specific City and Year
2. Show Top 10 Polluted Cities for a Year
3. Exit

Enter your choice (1/2/3): 1
Enter city (e.g., Delhi): Delhi
Enter year (e.g., 2026): 2026
```

Output:

| Month | Predicted AQI | AQI Bucket |
| ----- | ------------- | ---------- |
| Jan   | 241.5         | Poor       |
| Feb   | 198.3         | Moderate   |
| ...   | ...           | ...        |

AQI bucket is determined using CPCB guidelines.

---

## 🧠 How AQI Bucket is Classified

| AQI Range | Category     |
| --------- | ------------ |
| 0–50      | Good         |
| 51–100    | Satisfactory |
| 101–200   | Moderate     |
| 201–300   | Poor         |
| 301–400   | Very Poor    |
| 401–500+  | Severe       |
---
### 📊 AQI Bucket Distribution

![AQI Bucket Distribution](https://github.com/SiddardhaShayini/Air-Quality-in-Indian-Cities/blob/main/screenshots/AQI%20Bucket%20Distribution.png)

---

### 🔝 Top 10 Most Polluted Cities (Median AQI)

![Top 10 Most Polluted Cities](https://github.com/SiddardhaShayini/Air-Quality-in-Indian-Cities/blob/main/screenshots/Top%2010%20Most%20Polluted%20Cities%20(Median%20AQI).png)

---

### 🌱 Top 10 Least Polluted Cities (Median AQI)

![Top 10 Least Polluted Cities](https://github.com/SiddardhaShayini/Air-Quality-in-Indian-Cities/blob/main/screenshots/Top%2010%20Least%20Polluted%20Cities%20(Median%20AQI).png)


## 📚 Future Enhancements

* ✅ Streamlit-based Web UI
* 🌍 Geo-Map AQI forecasting
* 🧠 Deep learning (LSTM) for time-series forecasting
* 🏥 Health advisory predictions based on AQI levels

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

-----

## ✍️ Author

- Siddardha Shayini

-----
