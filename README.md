# Cyptocurrencies
UCB Challenge: Use skills associated with unsupervised learning to create an analysis for clients who are preparing to get into the cryptocurrency market.

# Overview of Analysis
Preprocess the database, reducing the data dimension using Principal Component Analysis or PCA, clustering cryptocurrencies using K-Means AND visualizing classification results with 2D and 3D scatter plots are skills associated with unsupervised learning; In this project we are given the task to analyze a database of cryptocurrencies using the skills mentioned above to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

## Preprocessing the Data for Principal Component Analysis or PCA
The original dataset had 1252 cryptocurrencies or rows and 6 columns, we were able to reduce this to 532 cryptocurrencies or rows and 4 columns. We were able to do this by removing rows with cryptocurrencies that were not being traded, rows that have at least one null and rows that do not have coins being mined. We took out or dropped the IsTrading column and the CoimName column. 

IMAGE HERE!

## Reducing Data Dimensions Using Principal Component Analysis or PCA
Principal Component Analysis or PCA was utilized to reduce the dimensions to three principal components; A new DataFrame that includes the following columns, PC 1, PC 2, and PC 3 was created.

IMAGE HERE!

## Clustering Cryptocurrencies Using K-means
Using the new DataFrame that was created, an elbow curve using hvPlot to find the best value for K was created using the K-Means method iterating on k values from 1 to 10. Based on the elbow curve, the best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies. 

IMAGE HERE!

Another DataFrame that including predicted clusters and cryptocurrencies features was created. It has the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class. In this case, class would pertain correspond to the prediction, in terms of what cluster the cryptocurrency belongs to.

IMAGE HERE!

## Visualizing Cryptocurrencies Results
A 3D scatter plot was created based on the previous column.

IMAGE HERE.




