# 📈 Apple Stock Machine Learning Project

## Overview  
This project analyzes Apple’s stock data using machine learning.  
The main goals were:  
- Explore and clean the dataset  
- Visualize important patterns  
- Build models to predict stock movement (Up/Down)  
- Use regression to estimate the closing price  

---

## Dataset  
- **Source**: Apple stock prices (`apple_stock.csv`)  
- **Columns**: Date, Open, High, Low, Close, Adj Close, Volume  
- Added a new feature → **Price Change %**  
- Created a **Movement** label:  
  - `1` → Stock closed higher than it opened (Up)  
  - `0` → Stock closed lower than it opened (Down)  

---

## Methods  
- **Preprocessing**: Missing values handled, features scaled  
- **EDA**: Histograms, scatter plots, boxplots, heatmap  
- **Classification Models**:  
  - Logistic Regression  
  - Decision Tree  
  - KNN  
- **Regression Model**:  
  - Linear Regression  

---

## Results  
- **Classification (Up/Down)**:  
  - Logistic Regression predicted only “Up”  
  - KNN ~50% accuracy (close to random)  
  - Decision Tree overfitted (100% train accuracy)  
  - → Shows predicting daily movement is difficult  

- **Regression (Close price)**:  
  - Linear Regression performed very well  
  - **MAE ~ $0.15**, **RMSE ~ $0.30**  
  - Captured price trends accurately  

---

## Conclusion  
- Daily stock movement prediction is unreliable with basic models  
- Regression on price works much better and gives very low error  
- Project highlights the difference between **classification vs regression** in stock analysis  

---

## How to Run  
1. Clone this repo:  
   ```bash
   git clone https://github.com/Manav-goel-07/TDS-ML-Project.git
2. Open in VS Code or Jupyter Notebook
3. Run the notebook tds_project.ipynb step by step
