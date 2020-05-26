# neuralNetwork - Determine which projects likely to be a success and will receive future funding

## Brief Summary

### Target: IS_SUCCESSFUL Column

### Pre-processing:
To remove data that are insignificant to the model, I removed all rows are no longer active (STATUS != 1). I also removed rows who are historically non-successful. During the initial modeling, I am not able to get accuracy score higher that 58% when non-successful data were included. Increasing number of hidden layer ( I increased up to 3 layer), increasing epoch value, and changing activation layers - all did not help in increasing predictive accuracy of more than 58%.

I also dropped EIN, Name, Special Considerations columns from the data.

### Model, Train, Evaluate
I used 1 hidden layer with 4 neurons in my model. Anything more than that did not result in any improvements or performance. I initially set my model to 2 layers with 24 and 12 neurons, however, there is no noticeable difference between that and my final model.

### Alternative Model
If I was to implement a differenc emodel, I will use Random Forest Classifier. It's output is similar to that of Neural network model, and was able to predict values in less than the time it did with neural network. 
