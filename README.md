# CS-725_Project_Algorithmic_Trading

## **Overview**

This project develops an **algorithmic trading strategy** designed for **mid to long-term investments**, leveraging **fundamental analysis** and **machine learning techniques**. After extensive experimentation with models such as **Linear Regression**, **Recurrent Neural Networks (RNNs)**, and **Bidirectional Long Short-Term Memory Networks (Bi-LSTMs)**, we concluded that **Bidirectional LSTMs** provide superior performance for stock price prediction tasks.

## **License**

This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for more details.

## **Team Members**
- Veenu Chhabra (24M2135)
- Farhan Jawaid (24M0801)
- Ravi Sah (24M0854)
- Thibault Magnin (24V0016)

## **Project Features**

- **Linear Regression Model**: Stock price prediction using linear regression with data transformations and regularization techniques.
- **Recurrent Neural Network (RNN) Model**: Stock price prediction using an RNN with three layers, dropout for regularization, and optimized loss functions.
- **Bidirectional LSTM Model**: Stock price prediction using a three-layer Bi-LSTM model with dropout and optimization techniques, outperforming both RNN and Linear Regression models.

---

## Filters

The function `filter_companies` applies the following filters:

1. **Price-to-Earnings (P/E) Ratio**:
   - A measure of a company's valuation relative to its earnings.
   - Filters companies with a `P/E Ratio` **greater than or equal to** the specified threshold (`pe`).

2. **Price-to-Book (P/B) Ratio**:
   - Indicates the valuation of a company relative to its book value.
   - Filters companies with a `Price-to-Book Ratio` **less than** the specified threshold (`pb`).

3. **Return on Equity (ROE)**:
   - A measure of financial performance, calculated as net income divided by shareholders' equity.
   - Filters companies with `ROE` **greater than** the specified threshold (`roe`).

4. **Earnings Per Share (EPS)**:
   - Indicates profitability per share of a company.
   - Filters companies with `EPS` **greater than** the specified threshold (`eps`).

5. **Debt-to-Equity (D/E) Ratio**:
   - Assesses a company's financial leverage.
   - Filters companies with a `Debt/Equity` ratio **less than** the specified threshold (`de`). 
   - Companies with `Debt/Equity` data missing (e.g., `NaN`) are also included in the results.

---

## Usage

The script is designed to process three categories of stocks: **large-cap**, **mid-cap**, and **small-cap**. Here are the specific thresholds used for each category:

### Large-Cap Stocks
- `P/E Ratio ≥ -10`
- `P/B Ratio < 10`
- `ROE > 0`
- `EPS > 10`
- `Debt/Equity < 70`

### Mid-Cap Stocks
- `P/E Ratio ≥ -10`
- `P/B Ratio < 12`
- `ROE > 0`
- `EPS > 6`
- `Debt/Equity < 70`

### Small-Cap Stocks
- `P/E Ratio ≥ 15`
- `P/B Ratio < 50`
- `ROE > 0`
- `EPS > 3`
- `Debt/Equity < 60`

---

## **Files and Descriptions**

- **Linear_regression_to_predict_stock_price.ipynb**: Implements a Linear Regression model for stock price prediction using data transformations and regularization techniques.
  
- **Stock_price_prediction_using_RNN.ipynb**: Implements an RNN-based model for stock price prediction, utilizing:
  - Three layers
  - Dropout for regularization
  - Optimized loss functions

- **Algorithmic_Trading.ipynb**: Implements a **Bidirectional LSTM-based model** for stock price prediction with:
  - Three Bidirectional LSTM layers
  - Dropout and optimized loss functions
  - Superior performance compared to RNNs and Linear Regression

## **Conclusion**

Bidirectional LSTMs outperform RNNs and Linear Regression models in stock price prediction tasks. Their ability to capture both **past and future dependencies** in time series data makes them particularly suitable for algorithmic trading strategies.

## **How to Use the Project**

### **Prerequisites**
- Python 3.8+ 
- Required libraries (install via pip):
  ```bash
  pip install -r requirements.txt
  ```

### **Instructions**
1. Clone the repository:
   ```bash
   git clone https://github.com/gods-gift/CS-725_Project_Algorithmic_Trading.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd CS-725_Project_Algorithmic_Trading
   ```

3. Open the respective Jupyter Notebooks in your IDE (e.g., Jupyter Notebook, VSCode):
   - `Linear_regression_to_predict_stock_price.ipynb`
   - `Stock_price_prediction_using_RNN.ipynb`
   - `Algorithmic_Trading.ipynb`
   
4. Run the notebooks and analyze the outputs.

## **Technologies Used**
- **Programming Language**: Python
- **Libraries**: NumPy, Pandas, Torch, Scikit-learn, Matplotlib, yfinance
- **Models**: Linear Regression, RNNs, Bidirectional LSTMs

## **Future Work**
- Fine-tuning hyperparameters for Bidirectional LSTM models
- Incorporating real-time stock market data streams for live predictions
- Exploring additional features for enhanced prediction accuracy

---

