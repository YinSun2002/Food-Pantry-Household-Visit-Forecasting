# Food Pantry Household Visit Forecasting
Our dataset contains 336 samples which contains number of client visit in Lakeview FP, number of COVID affected in Lee county, CPI, unemployment rate, average personal income, number of school open days and date of the client visit in every week. 

Based on the observation of 4 weeks of the data, our goal is to predict the number of client visit next week. In this prediction problem, the dataset is split into 80% of the training data and 20% of the inference data. 

# Procedure 1
The predictors used in this experiment are listed as follows:

1. Linear Regression 
2. LASSO (Regularization Parameter = 0.01)
3. Neural Network Based Regression (One Hidden Layer with 100 ReLU nodes)
4. Gradient Boosting (Max Depth 11)
5. Decision Tree Regression (Max Depth 19)
6. Bayesian Ridge Regression
7. Ridge Regression (Regularization Parameter 0.5)
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
| LASSO | 40.16% | 43.35% | 24.7%| 26.6%|
| Neural Network Based Regression | 33.91% | 44.13% | 24.5% | 25.67%|
| Gradient Boosting | 0% | 38.44% | 19.11% | 26.6 %|
| Decision Tree Regression|  0% | 41.98 %| 25.42% | 26.51%|
|Bayesian Ridge| 43.07% | 42.36%| 25.43% | 26.4%|
|Ridge Regression| 41.8% | 41.6%| 25.4% | 26.62% |
|Baseline Algorithm 1| | 71.4%| | |
|Baseline Algorhtm 2| |57%| | |



