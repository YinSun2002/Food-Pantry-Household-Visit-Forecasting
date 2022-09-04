# Food-Pantry-Household-Visit-Forecasting
Our dataset contains 336 samples which contains number of client visit in Lakeview FP, number of COVID affected in Lee county, CPI, unemployment rate, average personal income, number of school open days and date of the client visit in every week. 

Based on the observation of 4 weeks of the data, our goal is to predict the number of client visit next week. In this prediction problem, the dataset is split into 80% of the training data and 20% of the inference data. The predictors used in this experiment are listed as follows:

1. Linear Regression 
2. LASSO 
3. Neural Network Based Regression\
4. Gradient Boosting
5. Decision Tree Regression
6. Bayesian Ridge Regression
7. Ridge Regression
8. Naive Algorithm 1: The number of visits 2 months ago
9. Naive Algorithm 2: The average number of visits during the last two months


	
| Model | Test Size | AP<sup>test</sup> | AP<sub>50</sub><sup>test</sup> | AP<sub>75</sub><sup>test</sup> | batch 1 fps | batch 32 average time |
| :-- | :-: | :-: | :-: | :-: | :-: | :-: |
| [**YOLOv7**](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt) | 640 | **51.4%** | **69.7%** | **55.9%** | 161 *fps* | 2.8 *ms* |
| [**YOLOv7-X**](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7x.pt) | 640 | **53.1%** | **71.2%** | **57.8%** | 114 *fps* | 4.3 *ms* |
|  |  |  |  |  |  |  |
| [**YOLOv7-W6**](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-w6.pt) | 1280 | **54.9%** | **72.6%** | **60.1%** | 84 *fps* | 7.6 *ms* |
| [**YOLOv7-E6**](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-e6.pt) | 1280 | **56.0%** | **73.5%** | **61.2%** | 56 *fps* | 12.3 *ms* |
| [**YOLOv7-D6**](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-d6.pt) | 1280 | **56.6%** | **74.0%** | **61.8%** | 44 *fps* | 15.0 *ms* |
| [**YOLOv7-E6E**](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-e6e.pt) | 1280 | **56.8%** | **74.4%** | **62.1%** | 36 *fps* | 18.7 *ms* |
