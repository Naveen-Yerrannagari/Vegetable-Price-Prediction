# 🥕 Vegetable Price Prediction

A machine learning project to predict the **price per kg** of vegetables based on environmental conditions, seasonality, and product condition using various regression techniques including **Linear Regression**, **Support Vector Machine (SVM)**, and **Random Forest Regressor**.

---

## 📊 Dataset Overview

The dataset contains information about vegetables collected from a local market, with the following features:

- `Vegetable`: Type of vegetable (e.g., tomato, potato, cucumber)
- `Season`: Seasonal category (e.g., summer, winter)
- `Month`: Month of observation
- `Temp`: Average temperature
- `Deasaster Happen in last 3month`: Whether a natural disaster occurred recently
- `Vegetable condition`: Quality (e.g., fresh, average, scrap)
- `Price per kg`: Target variable

---

## 🔧 Preprocessing Steps

- **Data Cleaning**: Fixed typos (e.g., `"scarp"` → `"scrap"`)
- **Handling Missing Values**: Replaced blank or missing months with mode
- **Encoding**: Used one-hot encoding for categorical variables and ordinal encoding for months
- **Train-Test Split**: 70% training, 30% testing

---

## 📈 Models & Performance

| Model                 | R² Score | Mean Squared Error |
|----------------------|----------|--------------------|
| Linear Regression     | 0.81     | 582.61             |
| Support Vector Machine (SVM) | 0.19     | 3430.13            |
| Random Forest Regressor | **0.91**     | **271.64**             |

✅ **Random Forest** performs best in both R² and MSE.

---

## 🚀 Installation & Run Locally

1. Clone this repo:

   ```bash
   git clone https://github.com/your-username/vegetable-price-prediction.git
   cd vegetable-price-prediction
2. Install dependencies:

  ```bash
  pip install -r requirements.txt
```  

3. Run the notebook:
 ```bash
  jupyter notebook
```

## 🛠️ Tools Used
Python

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

Jupyter Notebook

# 📌 Key Takeaways
Vegetable pricing is influenced by seasonal and environmental factors.

Machine learning can effectively forecast prices with relatively small datasets.

Feature encoding plays a crucial role in model accuracy.

# 📸 Sample Visualization

Feature correlation for better understanding input relationships

