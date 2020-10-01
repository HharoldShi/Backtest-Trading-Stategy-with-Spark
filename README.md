# Backtest-Trading-Stategy-with-Spark
The system performs backtesting on the SMA (simple moving average) trading strategy. It mimics the process of buy and sell of stocks on numerous daily historical stock prices data. 

It leverages Spark to implement parallel processing to enhance execution efficiency. In detail, Spark Dataframe is used to read, sort, filter and update schema of the stock data. Spark RDD is utilized to map data into a series of time windows, and then the average stock price is calculated for each window, which forms the simple moving averages. 

An interactive interface is built with ipywidgets. On the interface, users are able to choose a stock to test and modify SMA parameters (fast and slow window sizes). The corresponding test results such as total profits, the number of transactions are displayed. The orginal stock prices along with SMAs are plotted in charts. 
