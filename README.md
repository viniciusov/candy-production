## About

This repository is related to the [Candy Production Dataset](https://www.kaggle.com/rtatman/us-candy-production-by-month).  
In this dataset, is given the US Candy Production by Month ([candy_production.csv](https://github.com/viniciusov/candy-production/blob/master/candy_production.csv)).

## Analysis

Plotting the US Candy Production by Month and the Monthly production, it's easy to see that we have a seasonality in this data.  
Thus, I splitted the data set into a Train and a Test set, keeping the last 12 months as an unseen data for this last one.

When you talk about time series predictions, there are two main cells that can deliver good results in a RNN (Recurrent Neural Network).
They are the **LSTM** (Long Short Term Memory) and the **GRU** (Gated recurrent units).

Dealing with these two different cells, it's expected to get 2 different results (predictions), so I thought it'd be better to make to separated analysis.

You can check them here:
- **LSTM**: [LSTM Jupyter-notebook](https://nbviewer.jupyter.org/github/viniciusov/candy-production/blob/master/candy_prediction_gridsearch_lstm.ipynb)
- **GRU**: [GRU Jupyter-notebook](https://nbviewer.jupyter.org/github/viniciusov/candy-production/blob/master/candy_prediction_gridsearch_gru.ipynb)

## Results

The final results are pretty good for simple RNN networks, showing that is possible to predict the production with good accuracy.

**LSTM**:  
![LSTM](https://github.com/viniciusov/candy-production/blob/master/Results/lstm.png)

**GRU**:  
![GRU](https://github.com/viniciusov/candy-production/blob/master/Results/gru.png)

