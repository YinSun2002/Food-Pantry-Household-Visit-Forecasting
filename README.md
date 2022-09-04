# Food Pantry Household Visit Forecasting
Our dataset contains 336 samples which contains number of client visit in Lakeview FP, number of COVID affected in Lee county, CPI, unemployment rate, average personal income, number of school open days and date of the client visit in every week. 

Based on the observation of 4 weeks of the data, our goal is to predict the number of client visit next week. In this prediction problem, the dataset is split into 80% of the training data and 20% of the inference data. 

# Procedure 1
The predictors used in this experiment are listed as follows:

1. Linear Regression 
2. LASSO 
3. Neural Network Based Regression\
4. Gradient Boosting
5. Decision Tree Regression
6. Bayesian Ridge Regression
7. Ridge Regression
8. Naive Algorithm 1: The number of visits 2 months ago
9. Naive Algorithm 2: The average number of visits during the last two months


# Procedure 2
Data Generation Using Variational Auto Encoder (VAE):

By using 336 samples and a variational auto encoder, we have generated 835 more data samples. The total dataset is split into 80% for training and 20% for inference. The encoder network has one intermediate layer with 10 ReLU nodes and 2 output nodes. The output of the encoder is the input of the decoder. The decoder has one intermediate layer with 10 linear nodes. The loss function is the addition of reconstruction loss which is the cross-entropy loss and KL divergence loss. After that, we have used the above mentioned algorithms.


# Performance	
The performance is measured by using Mean Absolution Percentage Error (MAPE).
| Algorithm | Training Error | Inference Error | Training Error with VAE | Inference Error with VAE | 
| :-- | :-: | :-: | :-: | :-: | 
|Linear Regression| 38.06 %| 45.08 %| 25.45 % | 26.4 %|

