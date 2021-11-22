# Cryptocurrency Analysis

## Overview of Cryptocurrency Analysis 
A cryptocurrency is a digital or virtual currency that is secured by cryptography, which makes it nearly impossible to counterfeit or double-spend. The purpose of this analysis is to use unsupervised machine learning to examine a database of cryptocurrencies. From the analysis, I create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. 

I complete the following analysis to create a report: 
1. Preprocessing the Data 
2. Reducing Data Dimensions
3. Clustering Cryptocurrencies Using K-Means
4. Visualizing Cryptocurrencies Results 


## Results

### Clustering Cryptocurrencies Using K-Means: Elbow Curve

![ElbowCurve](https://github.com/ksung1923/cryptocurrencies/blob/899c2ecb8637091a242fb5720036e3d162d1d1b7/Resources/elbow.PNG)

I produced the elbow curve above using K-Means method and iterating on K values from 1 to 10. From the graph, we see the best K value appears to be 4, so I conclude to use 4 clusters to categorize the cryptocurrency data. 

### Visualizing Cryptocurrencies Results

#### 3D-Scatter with Clusters

![3DScatter](https://github.com/ksung1923/cryptocurrencies/blob/899c2ecb8637091a242fb5720036e3d162d1d1b7/Resources/3d_scatter.PNG)

The 3D scatter plot above was created using the PCA algoritham. I reduced the crytocurrencies dimensions to three pricipal comonents. 

#### Table of Tradable Cryptocurrencies

![TradableTable](https://github.com/ksung1923/cryptocurrencies/blob/899c2ecb8637091a242fb5720036e3d162d1d1b7/Resources/tradable_table.PNG)

Above is a table with tradable cryptocurrencies that was created using the hvplot.table() function. 

#### 2D-Scatter with TotalCoinMined vs TotalCoinSupply 

![2DScatter](https://github.com/ksung1923/cryptocurrencies/blob/899c2ecb8637091a242fb5720036e3d162d1d1b7/Resources/2d_scatter.PNG)

The 2D scatter plot above was created using hvplot.scatter plot with x="TotalCoinsMined" and y="TotalCoinSupply". 

## Summary 
Following the preprocessing and cleaning phase the data has a total of 532 tradable cryptocurrencies.
