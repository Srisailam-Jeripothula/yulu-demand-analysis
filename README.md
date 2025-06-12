
# 🚲 Yulu Demand Forecasting – Statistical Case Study

This project analyzes ride-level electric cycle rental data from **Yulu**, a leading micro-mobility service provider in India, to identify patterns in demand based on working days, weather, and seasons. The goal is to help the company optimize its fleet distribution and improve revenue by leveraging statistical hypothesis testing and exploratory data analysis.

---

## 📊 Dataset Description

The dataset `yulu_data.csv` contains **10,886 records** representing hourly bike rental data. It includes weather conditions, temperature, time information, and user demand metrics.

### 🔢 Columns in the Dataset:

| Column Name | Description |
|-------------|-------------|
| `datetime` | Timestamp of the rental hour |
| `season` | Season (1: Spring, 2: Summer, 3: Fall, 4: Winter) |
| `holiday` | Boolean indicating if the day is a holiday |
| `workingday` | 1 if the day is a working day (not weekend or holiday), 0 otherwise |
| `weather` | Weather condition index (1: Clear, 2: Mist, 3: Light Rain, 4: Heavy Rain) |
| `temp` | Temperature in Celsius |
| `atemp` | "Feels-like" temperature in Celsius |
| `humidity` | Relative humidity |
| `windspeed` | Wind speed |
| `casual` | Number of non-registered users |
| `registered` | Number of registered users |
| `count` | Total bike rentals (casual + registered) |

---

## 🔍 Key Questions Addressed

- Does **working day status** significantly affect rental demand?
- Is rental demand **different across seasons and weather conditions**?
- Are **weather and season** dependent variables?
- What is the **distribution of rental activity across hours and days**?

---

## 🧪 Statistical Methods Used

- **2-Sample T-Test**: To test differences in rentals between working and non-working days.
- **One-Way ANOVA**: To compare means across multiple seasons and weather categories.
- **Chi-Square Test**: To check for independence between categorical predictors.
- **Assumption Testing**: Normality checks via **Q-Q plots** and **Shapiro-Wilk**, equality of variances via **Levene's Test**.

---

## 📈 Exploratory Data Analysis (EDA)

- Distribution analysis of rental activity by hour, day, and weather
- Correlation heatmaps between continuous variables
- Boxplots for seasonal and weather-based comparison
- Visual time-series demand pattern analysis

---

## 💡 Key Insights

- Rentals are **24% higher on working days** than non-working days (statistically significant).
- **Weather and season have a strong effect** on demand (ANOVA p < 0.001).
- Most orders happen in the **afternoon (13–18 hrs)**.
- Significant **dependency** found between season and weather via chi-square.

---

## 🛠️ Tech Stack

- **Language**: Python  
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, SciPy, Statsmodels  
- **Statistical Techniques**: T-Test, ANOVA, Chi-Square Test, Assumption Checking

---

## Author
[Srisailam Jeripothula](https://www.linkedin.com/in/srisailamjeripothula)
