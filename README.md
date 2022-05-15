# Cryptocurrencies

## Overview of the Analysis
Martha is a senior manager for the Advisory Services Team at Accountability Accounting, an important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked for help to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.

## Analysis Process 

###  Preprocessed the Data for PCA
Used Pandas to preprocess the dataset in order to perform PCA.

For more information on how this was done please see the [crypto_clustering](crypto_clustering.ipynb) file.

### Reduced Data Dimensions Using PCA 
Used nowledge of how to apply the Principal Component Analysis (PCA) algorithm to reduce the dimensions of the `X` DataFrame to three principal components and place these dimensions in a new DataFrame.

For more information on how this was done please see the [crypto_clustering](crypto_clustering.ipynb) file.

### Clustered Cryptocurrencies Using K-means
Used the K-means algorithm to create an elbow curve using hvPlot to find the best value for K from the `pcs_df` DataFrame. Then, ran the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.

For more information on how this was done please see the [crypto_clustering](crypto_clustering.ipynb) file.

### Visualized Cryptocurrencies Results
Created scatter plots with Plotly Express and hvplot to visualize the distinct groups that correspond to the three principal components from above, then created a table with all the currently tradable cryptocurrencies using the `hvplot.table()` function.

For more information on how this was done please see the [crypto_clustering](crypto_clustering.ipynb) file.
