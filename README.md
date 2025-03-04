# HousingPricePrediction_bb-assignment01



**House Price Prediction using PyTorch**

This project builds a regression model using PyTorch to predict house prices. The dataset used is the California Housing Dataset from sklearn.datasets. The target variable represents the median house price in $100,000s.

To preprocess the data, we normalize the features using StandardScaler and split the dataset into 80% training and 20% testing. The data is then converted into PyTorch tensors for model training. We experiment with two different activation functions—Sigmoid and ReLU—to compare their effectiveness in a regression setting.

The models are trained using the Adam optimizer and Mean Squared Error (MSE) loss function over 100 epochs. After training, we evaluate the models by computing their MSE on the test set and visualizing actual vs. predicted prices using scatter plots. The results show that ReLU outperforms Sigmoid for regression tasks, as Sigmoid restricts outputs between 0 and 1, making it unsuitable for predicting large values. On the other hand, ReLU enables the model to learn more effectively, leading to better performance and lower MSE.
