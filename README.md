# AI to Predict Yield in Aeroponics

This repository holds the code implemented in the two following papers:

1. "Ensemble Learning for Improving Generalization in Aeroponics Yield Prediction" being presented at the IEEE conference ISCAS 2020 in Spain.
2. "Interpretability of AI Models that use Data Fusion to Predict Yield in Aeroponics", currently under consideration.

# Ensemble Learning for Improving Generalization in Aeroponics Yield Prediction

The first part of this repository corresponds to the Python implementation for the first paper.

In this work, yield prediction in aeroponics is studied using ML. We have compared and analyzed three popular supervised ML methods - Dense Neural Network (DNN), Random Forest based on decision trees (RF) and Support Vector Regression (SVR). Air quality and water quality measurements including temperature, humidity, CO2 , pH and Total Dissolved Solids (TDS) are used for yield prediction. Other static inputs such as number of days before and after transplant are also used. Six crops are studied (garlic chives, basil, red chard, rainbow chard, arugula, and mint). DNN performs particularly well with the prediction. The root mean square error (MSE), mean absolute error (MAE) and coefficient of determination (R^2) are calculated to estimate the efficiency of the method. Mean square error and R^2 score of DNN are 0.10 and 0.67, RF follows DNN correctness with MSE and R^2
of 0.12 and 0.62, and SVR achieves 0.18 and 0.45 respectively, all of these values over the validation dataset. In addition to
individual models, the two top performing models are combined as an ensemble model to improve overall performance, which shows an average R^2 score over the whole dataset divided by crop of 0.81.

This part of the project contains 4 files (Jupyter notebooks): NeuralNetwork, RandomForest, and SupportVectorMachine have the code that trains those three models. The file named Predictions contains the code that generates the final results using the already trained models.

# Interpretability of AI Models that use Data Fusion to Predict Yield in Aeroponics

The second part of this repository corresponds to the Python implementation for the second paper (currently under consideration).

# Notes

1. Proper reference to the papers will be added once they are published.
2. The data used in this project is publicly available at: https://data.mendeley.com/datasets/wmyktpx9hv/1
