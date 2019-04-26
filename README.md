# Machine-Learning-Sosio
Stock Data Pricing
The sample stock data pricing : 
https://gist.github.com/codecraf8/2943bf6495fad245bb682fde5ef210b5

Retrieved the data from this and stored in CSV file.

The jupyter notebooks for stock market prediction using LSTM's.(Long Short Term Memory) has been uploaded.

The implementation is based on Datacamp Tutorial for stock market prediction.

The Dataset consists of 500000( 5 lakhs) entries .The training set is composed of 375000 entries and testing dataset is composed of 125000 entries.

The data normalization is done in terms of windows in order to get good normalized results in a smoothing_window_size of 90000 and training data ranging to 360000 entries.

Following Hyperparameters are used with in the model made with Tensorflow:
num_unrollings = 50 # Number of time steps you look into the future.
batch_size = 500 # Number of samples in a batch
num_nodes = [200,200,150] # Number of hidden nodes in each layer of the deep LSTM stack
n_layers = len(num_nodes) # number of layers
dropout = 0.2 # dropout amount (In order to reduce Model Overfitting).

Results: The model has been trained for 5 epochs due to lack of computation resources and the following are results obtained from the trained model.
Average loss at step 1: 0.078895
	Test MSE: 0.00544
	Finished Predictions
Average loss at step 2: 0.012456
	Test MSE: 0.00595
	Finished Predictions
Average loss at step 3: 0.011650
	Test MSE: 0.00539
	Finished Predictions
Average loss at step 4: 0.010453
	Test MSE: 0.00504
	Finished Predictions
Average loss at step 5: 0.010867
	Test MSE: 0.00470
	Finished Predictions
