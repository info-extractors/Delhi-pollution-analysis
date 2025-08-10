# Delhi Air Pollution Analysis and Prediction

---

## 🚀 Project Overview

This project delivers a comprehensive analysis of Delhi's air quality data with the goal to:

- Identify key pollutants that most significantly impact the Air Quality Index (AQI).
- Understand seasonal and weekly patterns in pollution levels.
- Develop a machine learning model to accurately predict AQI values.

---

## 📊 Key Findings & Insights

- **Seasonal Trend**  
  Air quality shows a clear cyclical pattern. AQI peaks in winter months (January & December) and improves during mid-year months.

- **Primary Pollutants**  
  Correlation analysis highlights the major contributors to high AQI levels:  
  - **PM2.5** (correlation ≈ 0.90)  
  - **PM10** (correlation ≈ 0.80)  
  - **Carbon Monoxide (CO)** (correlation ≈ 0.70)

- **Predictive Model Performance**  
  A Random Forest Regressor was trained with impressive results:  
  - **R² score:** 92.2% (explains most variance in AQI)  
  - **RMSE:** 31.05 (low error relative to data variability)

---

## 📂 Dataset Description

The dataset contains daily air quality measurements for Delhi with the following columns:

| Feature           | Description                                |
| ----------------- | ------------------------------------------|
| Date, Month, Year | Date information                          |
| Holidays_Count    | Number of holidays on a given day         |
| Days              | Day of the week (numerical encoding)      |
| PM2.5, PM10, NO2, SO2, CO, Ozone | Concentration levels of pollutants |
| AQI               | Air Quality Index (target variable)       |

---

## 🛠 Methodology

1. **Data Cleaning & Preparation**  
   - Loaded and cleaned the dataset  
   - Engineered features such as `Day_Name` and `PM2.5_to_PM10_Ratio`

2. **Exploratory Data Analysis (EDA)**  
   - Descriptive statistics and correlation analysis to reveal relationships

3. **Visualization**  
   - Created heatmaps, scatter plots, bar charts, and time series to visualize trends  
   - Examined effects of weekdays vs. weekends and holidays

4. **Predictive Modeling**  
   - Built and trained a Random Forest Regressor  
   - Evaluated model using R² score and RMSE metrics

---

## 🧰 Technologies Used

| Technology      | Purpose                                 |
| --------------- | ------------------------------------- |
| Python 3.x      | Programming language                   |
| Pandas          | Data manipulation and analysis        |
| Matplotlib      | Data visualization                    |
| Seaborn         | Advanced statistical plots             |
| Scikit-learn    | Machine learning modeling and evaluation |

---

## ⚙️ How to Run the Project

Follow these steps to reproduce the analysis:

```bash
# Clone this repository
git clone https://your-repository-url.git
cd your-project-directory

# Install dependencies
pip install -r requirements.txt

# Run the analysis
python your_analysis_script.py

python your_analysis_script.py
