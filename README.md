# Predicting Price Movements of an Exchange Traded Fund Using Neural Networks

This repository includes code, comments, and a report for the final project of UVA's SYS6016 Machine Learning course. 

The objective was to use neural networks to make predictions for future price movements for a stock on the NASDAQ exchange. This was a group project; however, the code and comments in this repository were written by me, Beni Shpringer. There was additional code written by other UVA students which is not included here, but is referenced in the final report.

The data provided gave events for the ETF _SOXX_, which tracks the semiconductor industry, on two days: 1/6/17, and the following trading day 1/9/17. The full dataset is not included in this repository due to a contractual agreement between UVA and the data provider.

My role in the project was to process the raw data into a cleaned dataset with additional features for use in neural networks, as well as create and tune a feedforward neural network that could be used for prediction.

The main contents of this repository are:
1. [Building the Order Book](https://github.com/bshpringer/neural-network-stock-prediction/blob/master/code/build_order_book.ipynb): in which I take the raw sequence of events, and build out bid and ask order books which are updated after each event. Several new features are created from the raw data in this notebook.
2. [Processing the Order Book for Use in Neural Networks](https://github.com/bshpringer/neural-network-stock-prediction/blob/master/code/neural_net.ipynb): in which I split the data into training, validation, and test sets, as well as standardize features, and encode labels for use in neural networks.
3. [Feedforward Neural Network](https://github.com/bshpringer/neural-network-stock-prediction/blob/master/code/neural_net.ipynb): in which I build, run, and tune a neural network using TensorFlow in order to make predictions based on the given data.
4. [Final Report](https://github.com/bshpringer/neural-network-stock-prediction/blob/master/info/Final_Report.pdf): in which we discuss the process, results, and conclusions of the project.

Also included are additional comments regarding some of the logic and features of the project:
* [Logic for OrderBook class methods](https://github.com/bshpringer/neural-network-stock-prediction/blob/master/info/OrderBook_Methods.ipynb)
* [Descriptions of Raw and Engineered Features](https://github.com/bshpringer/neural-network-stock-prediction/blob/master/info/Column_Descriptions.ipynb)
