# yield_aeroponics
Ensemble Learning for Improving Generalization in Aeroponics Yield Prediction

Python implementation of the code used in the paper "Ensemble Learning for Improving Generalization in Aeroponics Yield Prediction" that will be presented at the IEEE conference ISCAS 2020 in Spain.

In this work, yield prediction in aeroponics is studied using ML. We have compared and analyzed three popular supervised ML methods - Dense Neural Network (DNN), Random Forest based on decision trees (RF) and Support Vector Regression (SVR). Air quality and water quality measurements including temperature, humidity, CO2 , pH and Total Dissolved Solids (TDS) are used for yield prediction. Other static inputs such as number of days before and after transplant are also used. Six crops are studied (garlic chives, basil, red chard, rainbow chard, arugula, and mint). DNN performs particularly well with the prediction. The root mean square error (MSE), mean absolute error (MAE) and coefficient of determination (R^2) are calculated to estimate the efficiency of the method. Mean square error and R^2 score of DNN are 0.10 and 0.67, RF follows DNN correctness with MSE and R^2
of 0.12 and 0.62, and SVR achieves 0.18 and 0.45 respectively, all of these values over the validation dataset. In addition to
individual models, the two top performing models are combined as an ensemble model to improve overall performance, which shows an average R^2 score over the whole dataset divided by crop of 0.81.

This project contains 4 files (Jupyter notebooks): NeuralNetwork, RandomForest, and SupportVectorMachine have the code that trains those three models. The file named Predictions contains the code that generates the final results using the already trained models.

Proper reference to the paper will be added once it is published, and if possible the original dataset will be published.
