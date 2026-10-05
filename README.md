# Car Price Prediction using Linear Regression

## Project Overview
This project applies **Linear Regression** to predict automobile prices based on key performance and efficiency features.  
It demonstrates end‑to‑end data analysis, model building, and evaluation using Python and scikit‑learn.

---

## Objective
To build a regression model that explains how **engine size, horsepower, and highway‑mpg** influence car prices, and to evaluate its accuracy using standard metrics.

---

## Dataset
The dataset contains automobile specifications and prices, including:
- Engine size
- Horsepower
- Highway miles per gallon (mpg)
- Other attributes (make, body‑style, fuel system, etc.)

---
## Observations
Relation between horsepoower and price
<img width="616" height="542" alt="image" src="https://github.com/user-attachments/assets/b4063511-f82d-4b78-b99f-cdba1c36d90a" />


---

## Tech Stack
- **Python** (data analysis & modeling)
- **Pandas & NumPy** (data wrangling)
- **Matplotlib & Seaborn** (visualization)
- **Scikit‑learn** (linear regression, metrics)

---

## Workflow
1. **Data Exploration**  
   - Visualized relationships (horsepower vs. price, mpg vs. price).  
   - Hexbin and regression plots confirmed positive correlation with horsepower and negative correlation with mpg.

2. **Model Training**  
   - Features: `engine-size`, `horsepower`, `highway-mpg`  
   - Target: `price`  
   - Train/test split (70/30).  
   - Fitted Linear Regression model.

3. **Model Coefficients**
   | Feature       | Coefficient | Interpretation |
   |---------------|-------------|----------------|
   | Engine-size   | +125.82     | Larger engines increase price significantly. |
   | Horsepower    | +22.93      | Higher horsepower increases price moderately. |
   | Highway-mpg   | –146.95     | More fuel efficiency lowers price. |

4. **Model Evaluation**
   - **R²:** ~0.74–0.79 → explains ~79% of price variance.  
   - **MAE:** ~2,635 → average prediction error.  
   - **RMSE:** ~4,065 → typical error size in price units.
