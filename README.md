# AEFES Time Series Forecasting 📈

![GitHub release](https://img.shields.io/github/release/jasontan22/aefes-time-series-forecasting.svg)
![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![TensorFlow](https://img.shields.io/badge/tensorflow-2.4%2B-orange.svg)

Welcome to the AEFES Time Series Forecasting repository! This project uses market data from Anadolu Efes Biracılık ve Malt Sanayii A.Ş. (AEFES) to predict future closing prices using deep learning techniques such as LSTM, BiLSTM, and CNN+LSTM. 

You can find the latest releases of this project [here](https://github.com/jasontan22/aefes-time-series-forecasting/releases). Make sure to download the files and execute them for a hands-on experience.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Data Preprocessing](#data-preprocessing)
6. [Model Training](#model-training)
7. [Evaluation](#evaluation)
8. [Contributing](#contributing)
9. [License](#license)
10. [Contact](#contact)

## Project Overview

This project aims to forecast the closing prices of AEFES stocks. By utilizing deep learning models, we can analyze historical data and make informed predictions about future prices. The main components of the project include:

- Data collection and preprocessing
- Building and training models
- Evaluating model performance
- Making predictions

## Technologies Used

This project employs several technologies and libraries, including:

- **Python**: The main programming language for this project.
- **TensorFlow**: A powerful library for building and training deep learning models.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization.
- **Seaborn**: For statistical data visualization.

## Installation

To set up this project on your local machine, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/jasontan22/aefes-time-series-forecasting.git
   ```

2. Navigate to the project directory:

   ```bash
   cd aefes-time-series-forecasting
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

To use the forecasting models, you need to execute the main script. Here’s how to do it:

1. Open your terminal.
2. Navigate to the project directory if you haven’t already.
3. Run the script:

   ```bash
   python main.py
   ```

The script will execute the data preprocessing, model training, and evaluation steps automatically.

## Data Preprocessing

Data preprocessing is a crucial step in any machine learning project. In this project, we perform the following tasks:

1. **Data Collection**: We gather historical stock prices from a reliable source.
2. **Cleaning Data**: We handle missing values and remove any anomalies.
3. **Normalization**: We scale the data to improve model performance.
4. **Splitting Data**: We divide the dataset into training and testing sets.

The code for data preprocessing can be found in the `data_preprocessing.py` file.

## Model Training

In this project, we explore various deep learning models:

### LSTM (Long Short-Term Memory)

LSTM networks are effective for time series forecasting due to their ability to remember long-term dependencies. We build an LSTM model using TensorFlow.

### BiLSTM (Bidirectional LSTM)

BiLSTM extends LSTM by processing data in both forward and backward directions. This can capture more context from the data.

### CNN+LSTM

This model combines Convolutional Neural Networks (CNN) with LSTM to extract features from time series data before making predictions.

You can find the implementation details in the `model_training.py` file.

## Evaluation

After training the models, we evaluate their performance using metrics such as Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE). We visualize the predictions against actual values to assess the model's accuracy.

The evaluation code is located in the `evaluation.py` file.

## Contributing

We welcome contributions to improve this project. If you want to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push to your branch.
5. Create a pull request.

Please ensure your code adheres to the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, feel free to reach out:

- **Email**: your.email@example.com
- **GitHub**: [jasontan22](https://github.com/jasontan22)

You can find the latest releases of this project [here](https://github.com/jasontan22/aefes-time-series-forecasting/releases). Download the files and execute them to explore the capabilities of this forecasting model.

Thank you for visiting the AEFES Time Series Forecasting repository! Happy coding!