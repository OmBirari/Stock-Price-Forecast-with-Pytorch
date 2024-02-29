# Stock Price Forecast with PyTorch

This project utilizes PyTorch to implement a stock price forecasting model. The neural network architecture consists of three linear layers with ReLU activation functions. The dataset is preprocessed to include additional metrics such as moving averages and standard deviations.

## Model Architecture

The neural network model (`Model`) consists of three linear layers with 250, 100, and the desired output neurons, respectively. The Rectified Linear Unit (ReLU) activation function is applied between layers for non-linearity.

## Metrics and Preprocessing

The `AddMetrics` function calculates moving averages, lower bounds, and upper bounds to enhance the dataset. The `TrainTest` function splits the data into training and testing sets. The `Inputs` function prepares input-output pairs for training, and the `Outputs` function generates input data for prediction.

## Training

The model is trained for a specified number of epochs using Mean Squared Error Loss and the Adam optimizer. Training progress is displayed, and the final model is used to make predictions.

## Usage

1. Install required libraries: `numpy`, `pandas`, `torch`, and `matplotlib`.
2. Provide the stock data in CSV format (e.g., 'AAPL.csv').
3. Adjust parameters such as `epochs`, `window`, `output`, and `learning_rate` as needed.
4. Run the script to train the model and visualize predictions.

## Results<br>
The script plots historical stock prices and predicted values using matplotlib.

Feel free to experiment and contribute to further enhance the forecasting model.


