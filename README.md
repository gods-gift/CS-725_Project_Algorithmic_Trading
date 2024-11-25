#CS-725 Project: Algorithmic Trading

Overview
This project aims to develop an algorithmic trading strategy designed for mid and long-term investments by leveraging fundamental analysis and machine learning techniques. Through comprehensive experimentation with models such as Linear Regression, RNNs, and Bidirectional LSTMs, we concluded that Bidirectional LSTMs perform better for stock price prediction.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

Team Members
Veenu Chhabra (24M2135)
Farhan Jawaid (24M0801)
Ravi Sah (24M0854)
Thibault Magnin (24V0016)
Project Features
Linear Regression with data transformations and regularization for stock price prediction.
Recurrent Neural Networks (RNN) with dropout and optimization techniques, incorporating 3 layers to predict stock prices.
Bidirectional LSTM models with 3 layers, dropout, and optimization for improved prediction accuracy.
Files and Descriptions
Linear_regression_to_predict_stock_price.ipynb
Implements Linear Regression for stock price prediction with data transformations and regularization techniques.

Stock_price_prediction_using_RNN.ipynb
Demonstrates an RNN-based model with:

3 layers
Dropout for regularization
Optimized loss function
Algorithmic_Trading.ipynb
Implements a Bidirectional LSTM-based model with:

3 Bidirectional LSTM layers
Dropout and optimizer
Superior performance compared to RNN and Linear Regression
Conclusion
Bidirectional LSTMs outperform RNNs and Linear Regression in stock price prediction tasks.
Bidirectional LSTMs effectively capture both past and future dependencies in time series data, making them a robust choice for algorithmic trading strategies.
How to Use the Project
Prerequisites
Python 3.8+
Required libraries (install via pip):
bash
Copy code
pip install -r requirements.txt
Instructions
Clone the repository:

bash
Copy code
git clone https://github.com/gods-gift/CS-725_Project_Algorithmic_Trading.git
Navigate to the directory:

bash
Copy code
cd CS-725_Project_Algorithmic_Trading
Open the respective Jupyter Notebooks in your IDE (e.g., Jupyter Notebook, VSCode):

Linear_regression_to_predict_stock_price.ipynb
Stock_price_prediction_using_RNN.ipynb
Algorithmic_Trading.ipynb
Run the notebooks and analyze the outputs.

Technologies Used
Programming Language: Python
Libraries: NumPy, Pandas, PyTorch, Scikit-learn, Matplotlib
Models: Linear Regression, RNNs, Bidirectional LSTMs
Future Work
Fine-tuning hyperparameters for Bidirectional LSTM models.
Incorporating real-time stock market data streams.
Exploring additional features for enhanced prediction accuracy.
Contact
For questions or contributions, feel free to contact:

Veenu Chhabra: veenu.chhabra@example.com
Let me know if you need further changes!











ChatGPT can make mistakes.
