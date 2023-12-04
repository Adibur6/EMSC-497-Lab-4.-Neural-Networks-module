# EMSC-497-Lab-4.-Neural-Networks-module

## Task 1 - Classification

### Overview

In Task 1, we aimed to build and evaluate two different Convolutional Neural Network (CNN) structures for the handwritten digit classification problem using the MNIST dataset. The two CNN structures incorporated max-pooling and average-pooling layers, respectively. Additionally, we compared the performance of these CNN models with a tutorial CNN model.

### Models and Results

1.  **CNN_Max-pool**
    
    -   Accuracy: 98.79%
    -   Precision: 98.80%
    -   Recall: 98.79%
    -   F1 Score: 98.79%
    -   Loss: 0.0398
2.  **CNN_Avg-pool**
    
    -   Accuracy: 98.27%
    -   Precision: 98.29%
    -   Recall: 98.27%
    -   F1 Score: 98.27%
    -   Loss: 0.0588
3.  **Tutorial CNN**
    
    -   Accuracy: 99.50%
    -   Precision: 99.50%
    -   Recall: 99.50%
    -   F1 Score: 99.50%
    -   Loss: 0.0187

### Observations

-   The tutorial CNN achieved the highest accuracy among the three models.
-   CNN_Max-pool and CNN_Avg-pool demonstrated competitive performance, with CNN_Max-pool having a slightly better accuracy.

## Task 2 - Regression

### Overview

Task 2 involved predicting biodiversity ('bbsrich') using a neural network regression model. We utilized the biodiversity data from Lab 2, with variables 'JanMeanTem', 'JulyMeanTe', 'pptMean', 'seasMean', 'elevationM', 'elevationS', 'slopeMean', 'slopeStdev', 'lulcDecicu', 'lulcEvergr', 'lulcMixFor', 'lulcWater'. We split the data into 70% training and 30% test sets and experimented with different neural network models. We also compared the neural network models with a Random Forest regression model.

### Models and Results

1.  **NN Variation1**
    
    -   Training RMSE: 13.20
    -   Test RMSE: 14.54
    -   Training R2 Score: 0.799
    -   Test R2 Score: 0.761
2.  **NN Variation2**
    
    -   Training RMSE: 10.30
    -   Test RMSE: 13.24
    -   Training R2 Score: 0.878
    -   Test R2 Score: 0.802
3.  **NN Variation3**
    
    -   Training RMSE: 9.52
    -   Test RMSE: 14.12
    -   Training R2 Score: 0.895
    -   Test R2 Score: 0.775
4.  **Random Forest**
    
    -   Training RMSE: 4.91
    -   Test RMSE: 12.71
    -   Training R2 Score: 0.972
    -   Test R2 Score: 0.818

### Observations

-   NN Variation2 performed the best among the neural network models in terms of both RMSE and R2 Score.
-   Random Forest outperformed all neural network models in terms of Test R2 Score, suggesting its effectiveness for this regression task.
-   Overfitting concerns were observed, especially in NN Variation1, where the training RMSE was substantially higher than the test RMSE.

## Conclusion

-   For classification tasks, the tutorial CNN demonstrated superior performance, but both CNN_Max-pool and CNN_Avg-pool provided competitive results.
-   In regression tasks, careful consideration of model complexity is crucial to avoid overfitting. Random Forest proved effective in handling the complexity of the biodiversity prediction task.

Feel free to explore the provided code for detailed implementations and analyses.
