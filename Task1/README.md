# CodeAlpha_Stock_Prediciton
Stock Price Prediction with LSTM

This project aims to predict stock prices using Long Short-Term Memory (LSTM) neural networks. The LSTM model is trained on historical stock data to forecast future stock prices. Here's an overview of the process:
Dataset

I used historical stock data of Microsoft Corporation obtained from Kaggle. The dataset contains various features such as high, low, open, close prices, volume, and adjusted close.
Implementation

    Data Preprocessing: The dataset is preprocessed by handling missing values, removing outliers, and normalizing numerical features using MinMaxScaler.
    Model Building: An LSTM model is constructed using TensorFlow's Keras API. The model architecture consists of one LSTM layer followed by a dense layer.
    Model Training: The model is trained on the preprocessed data with a validation split of 20%. The training process involves optimizing the mean squared error loss using the Adam optimizer.
    Model Evaluation: The trained model is evaluated on the testing set, and the root mean squared error (RMSE) is calculated to assess its performance.
    Results Visualization: Actual vs. predicted stock prices are plotted to visually inspect the model's performance.

Usage

To run the code:

    Install the required libraries using pip install -r requirements.txt.
    Ensure the dataset (Microsoft Corporationstock.csv) is in the same directory.
    Run the code in your Python environment.

Results

The LSTM model demonstrates promising performance with an RMSE of 0.007. The visualization shows that the predicted stock prices closely follow the actual prices, indicating the model's effectiveness in capturing the underlying patterns in the data.
